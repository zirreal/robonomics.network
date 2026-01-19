<template>
  <gsp-form
    :gscriptID="gscript"
    :siteKey="siteKey"
    @gsp-beforesubmit="beforeSubmit"
    @gsp-onsubmit="onSubmit"
    @gsp-oncaptchanotverified="captchaError"
  >
    <input
      type="text"
      data-gsp-name="Name"
      :data-gsp-data="name"
      v-model="name"
      :placeholder="$tr('Your name')"
      class="block"
      required
    />

    <input
      type="email"
      data-gsp-name="Email"
      :data-gsp-data="email"
      v-model="email"
      :placeholder="$tr('Your email')"
      class="block"
      required
    />

    <textarea
      data-gsp-name="Comment"
      :data-gsp-data="message"
      v-model="message"
      :placeholder="$tr('Your message')"
      class="block"
    ></textarea>

    <input type="hidden" data-gsp-name="Location" :data-gsp-data="location" />
    <input type="hidden" data-gsp-name="Tags" :data-gsp-data="tags.toString()" />

    <RoboButton 
      class="block"
      :loading="status === 'process'"
      :type="buttontype">
      {{ buttontext }}
    </RoboButton>

    <span class="text-small error" v-if="errorMessage">{{ errorMessage }}</span>
  </gsp-form>
</template>

<script setup>
import { ref, computed, defineAsyncComponent } from 'vue';
import { translateVue as $tr} from '../../assets/scripts/utils/translate';

import RoboButton from '../utils/Button.vue';
const GspForm = defineAsyncComponent(() => import('../utils/Form.vue'));

const name = ref('');
const email = ref('');
const message = ref('');
const location = ref(window.location.href);
const gscript = ref(import.meta.env.PUBLIC_CONTACTS_FORM_SCRIPT);
const siteKey = ref(import.meta.env.PUBLIC_RECAPTCHA);
const status = ref('init');
const tags = ref(['contact-form']);
const errorMessage = ref('');

const buttontype = computed(() => ({
  'ok': 'ok',
  'error': 'error',
  'na': 'na',
}[status.value] ?? 'primary'));

const buttontext = computed(() => ({
  'ok': $tr('Thanks for the submission!'),
  'error': $tr('Not submitted'),
  'process': $tr('Submitting'),
}[status.value] ?? $tr('SEND')));

const captchaError = () => {
  status.value = 'na';
  errorMessage.value = $tr('Captcha is not verified. Please, check your internet connection');
};

const beforeSubmit = () => {
  status.value = 'process';
  errorMessage.value = '';
};

const onSubmit = (response) => {
  status.value = response.result === 'success' ? 'ok' : 'error';
  if(status.value === 'error') {
    errorMessage.value = response.message
  } else if (status.value === 'ok') {
    // Reset form on success
    name.value = '';
    email.value = '';
    message.value = '';
  }
};
</script>

<style scoped>
:deep(gsp-form) {
  text-align: center;
}

input::placeholder, textarea::placeholder {
  font-variation-settings: var(--font-flex-italic);
}

textarea.block {
  margin-bottom: var(--space);
  width: 100%;
  min-height: 120px;
  resize: none;
  border-radius: 6px;
}

.error {
  display: inline-block;
  margin-top: calc(var(--space) * 0.5);
  line-height: 1.2;
  color: var(--color-red);
  text-align: center;
}
</style>

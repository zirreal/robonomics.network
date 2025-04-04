<template>
  <layout>

    <MetaInfo
      pageTitle = "Crowdloan for Robonomics on Kusama"
      pageDescription = "Crowdloan Description"
      pageImage = "/website_cover_crowdloan.jpg"
      pageImageHeight = "652"
    />

    <div class="page">
       <section id="info" class="section__solid section__blue">
         <div class="content layout laouyt__content">
           <h1>{{$ts('Robonomics won parachain slot on Kusama')}}</h1>
           <p id="info-subtitle">{{$ts('Dotsama for robots program initiated')}} <g-link to="/blog/parachain-on-kusama-first-week-report/">{{$ts('Read first report')}}</g-link></p>

           <div class="grid-3">
             <div class="oldy dark bg-blue align-left">
               <div class="text-title">{{$ts('Global parameters')}}</div>
               <div class="text-small">
                  <p><b>{{$ts('Auction:')}}</b> 20</p>
                  <p><b>{{$ts('Lease Period:')}}</b> 18 - 25</p>
                  <p><b>{{$ts('Retroactive Auction Ending Block:')}}</b> 10,751,100</p>
                  <p><b>{{$ts('Last valid contribution block:')}}</b> 10,784,569</p>
                  <p><b>{{$ts('Best Bid:')}}</b> 13,236 $KSM</p>
                  <p><g-link to="https://kusama.subscan.io/bid_history/?bid_id=20-18-25"><b>{{$ts('Check status of your bid on Subscan')}}</b></g-link></p>
               </div>
             </div>

             <div class="oldy dark bg-blue align-left">
               <div class="text-title">{{$ts('Remuneration summary')}}</div>
               <div class="text-small">
                  <p>{{$ts('4.20 XRT each KSM')}}</p>
                  <p>{{$ts('1 XRT extra each KSM for')}} <g-link to="https://opensea.io/assets/0xdc9fe731ce957c14a7b055a34270b2400b0905ec/1">«{{$ts('Pioneer NFT')}}»</g-link> {{$ts('cardholders')}}</p>
                  <p>+ {{$ts('Robonomics Pioneer NFT for all contributors')}}</p>
                  <p><g-link to="https://app.subsocial.network/@rmrkapp/robonomics-partnership-rmrk-goes-robotic-beep-boop-28764"><b>+ {{$ts('Robonomics Kanaria Collection')}}</b></g-link> {{$ts('for 500 top contributors')}}</p>
               </div>
             </div>

             <div class="oldy dark bg-blue align-left">
               <div class="text-title">{{$ts('Plans')}}</div>
               <div class="text-small">
                  <p>{{$ts('Robonomics will be onboarded in ~2 weeks')}}</p>
                  <p>{{$ts('We will focus on Kusama apps for IoT startups and smart home infrastructure, read more')}} <g-link to="/blog/trajectory-2022-heading-for-product-launches/">{{$ts('here')}}</g-link></p>
                  <p>{{$ts('Monthly IoT subscriptions for your home infrastructure will be available before end of the month with start price 0.5 XRT.')}} <g-link to="https://www.youtube.com/watch?v=H-w2FX-zd0M">{{$ts('Have a look on example')}}</g-link></p>
               </div>
             </div>
           </div>

           <g-image id="info-girl" aria-hidden="true" alt="" src="~/assets/images/kusama-cosmogirl-sitting.png" quality="75" />

         </div>
         
         <div id="info-numbers">
           <MovingNumbers/>
         </div>
       </section>

       <section id="a-contribution" class="section__solid section__darkgray">

         <div class="contribution layout">
           <h3>{{$ts('Subscribe to email news & updates')}}</h3>
           <Subscribtion />
         </div>
       </section>

       <section class="layout layout__text">
         <h2>{{$ts('Quick intro to Robonomics')}}</h2>

         <div class="oldy-wrap-count">
           <section class="oldy dark">
            <div class="oldy-count-content">
              {{$ts('Robonomics is an open-source platform for IoT applications. We support a new generation of internet technologies (Web3) that implements the exchange of technical and economic information in the form of atomic transactions between user applications, IoT services, and complex robotics.')}}
            </div>
          </section>

           <section class="oldy dark">
            <div class="oldy-count-content">
              {{$ts('The Robonomics project is over 6 years old. We started to prepare for the first experiment demonstrating human-machine communication using an independent decentralized provider network in 2015, from the early days of the Ethereum network. By early 2021, the project team managed to create a techno-economic machine communication protocol running on top of Ethereum and IPFS, and complement it with elements of a cloud-based IoT platform based on the Polkadot parachain.')}}
            </div>
          </section>

          <section class="oldy dark">
            <div class="oldy-count-content">
              {{$ts('Robonomics contains a complete set of tools for developing IoT applications, both on the robotics and the user interface sides. Communication between the user and device happens using the most successful technologies from the Web3 world – IPFS, Ethereum, and Polkadot. Thus, developers can create modern and secure applications for Smart Cities and Industry 4.0.')}}
            </div>
          </section>

          <section class="oldy dark">
            <div class="oldy-count-content">
              {{$ts('We are launching Robonomics Web Services. This sustainable subscription model for IoT devices makes possible to execute zero-weight transactions in blockchain.')}}
            </div>
          </section>
         </div>

         <a href="#a-contribution" class="dashed text-big" v-smooth-scroll="{ updateHistory: false, offset: -250 }">{{$ts('Email updates')}}</a>
       </section>

      <section class="section__solid section__lightblue animate" v-in-viewport.once>
        <h2>{{$ts('Robonomics in Polkadot ecosystem')}}</h2>

        <div class="grid-3 layout layout__content">

        <Card orientation="vertical" back="transparent" link="https://youtu.be/rbjOmJmilAg">

          <p>
            <g-image alt="Video from Polkadot Decoded 2021" src="~/assets/images/Sergei-Polkadot-may-2021.png"/>
          </p>

          <h3>{{$ts('Polkadot Decoded 2021')}}</h3>
          <p class="hyphens">{{$ts('On May 19, on the main stage of Polkadot Decoded, Sergey Lonshakov spoke about the concept of Smart cities and Polkadot services that are possible within this.')}}</p>

        </Card>

        <Card orientation="vertical" back="transparent" link="https://youtu.be/31zXeUq3htE">

          <p>
            <g-image alt="Kusama on Mars video" src="~/assets/images/Kusama-On-Mars.png"/>
          </p>

          <h3>{{$ts('Kusama on Mars')}}</h3>
          <p class="hyphens">{{$ts('On Hackusama (a 7-week online hackathon) we inspired with an idea of architecture impossible without KUSAMA. Watch the video and read in the description what was done during the hackathon.')}}</p>

        </Card>

        <Card orientation="vertical" back="transparent" link="https://opensea.io/assets/0x8cb813bf27dc744fc5fb6ba7515504de45d39e08/24">

          <p>
            <g-image alt="Robonomics PolkaPet" src="~/assets/images/robonomics-nft-3.png"/>
          </p>

          <h3>{{$ts('Robonomics PolkaPet')}}</h3>
          <p class="hyphens">{{$ts('PolkaPet is collectible NFT card embodied as an artistic creature, represents a specific project within the Polkadot ecosystem. Robonomics PolkaPets owners can get some additional bonuses.')}}</p>

        </Card>

        </div>
      </section>

      <hr class="animate no-margins" v-in-viewport.once/>

      <section class="parachain animate" v-in-viewport.once>
        <section class="parachain-intro section__solid section__gradient-purpleblue">
          <div class="layout layout__text animate-inside" v-in-viewport.once>
            <h2>{{$ts('Why parachain')}}</h2>
            <p class="hyphens">{{$ts('Kusama parachain is great opportunity for Robonomics to scale network up to 1 million IoT systems connected in real-time without any centrilized regulators.')}}</p>
            <p class="hyphens">{{$ts('The Robonomics developers team formed plan for 2 years within Kusama slot. We will try to build on our existing work and new software development 5 specific features, including')}}:</p>

            <div class="parachains-overview">

              <div class="parachains-overview-description">

                <div class="item" :class="(parachainTab == 1) ?'active':''">
                  <h4>{{$ts('Smart leasing')}}</h4>
                  <p class="hyphens">{{$ts('Recoup your investment in the high-value robots by renting out it with a mechanism for tokenizing robots’ labor.')}}</p>
                </div>
                <div class="item" :class="(parachainTab == 2) ?'active':''">
                  <h4>{{$ts('Robot as a Service (RaaS)')}}</h4>
                  <p class="hyphens">{{$ts('Get and provide direct robot services without cashiers, clerks or centrilized cloud providers.')}}</p>
                </div>
                <div class="item" :class="(parachainTab == 3) ?'active':''">
                  <h4>RWS</h4>
                  <p class="hyphens">{{$ts('Robonomics Web Services (RWS) will provide decentralized infrastructure for IoT solutions.')}}</p>
                </div>
                <div class="item" :class="(parachainTab == 4) ?'active':''">
                  <h4>DAO IPCI</h4>
                  <p class="hyphens">{{$ts('The Robonomics network provides technology for environmental mitigation service DAO IPCI.')}}</p>
                </div>
                <div class="item" :class="(parachainTab == 5) ?'active':''">
                  <h4>Distributed Sky</h4>
                  <p class="hyphens">{{$ts('Blockchain techonologies to control the traffic of drones (automated planning of drone flight paths, decentralized payment regulations, smart contract for transactions)')}}</p>
                </div>

              </div>

               <div class="parachains-overview-line">

                  <div class="item" :class="(parachainTab == 1) ?'active':''" @click="parachainTab=1">
                    <g-image src="~/assets/images/parachain-i-leasing.png" />
                    <p class="item-title">{{$ts('Smart rental and leasing')}}</p>
                  </div>

                  <div class="item" :class="(parachainTab == 2) ?'active':''" @click="parachainTab=2">
                    <g-image src="~/assets/images/parachain-i-robot-as-a-service.png" />
                    <p class="item-title">{{$ts('Robot as a Service')}}</p>
                  </div>

                  <div class="item" :class="(parachainTab == 3) ?'active':''" @click="parachainTab=3">
                    <g-image src="~/assets/images/parachain-i-rws.png" />
                    <p class="item-title">{{$ts('"Cloud" for IoT applications')}}</p>
                  </div>

                  <div class="item" :class="(parachainTab == 4) ?'active':''" @click="parachainTab=4">
                    <g-image src="~/assets/images/parachain-i-enviromental.png" />
                    <p class="item-title">{{$ts('Environmental mitigation')}}</p>
                  </div>

                  <div class="item" :class="(parachainTab == 5) ?'active':''" @click="parachainTab=5">
                    <g-image src="~/assets/images/parachain-i-drones-traffic.png" />
                    <p class="item-title">{{$ts('Drone vehicle traffic')}}</p>
                  </div>

              </div>


            </div>
          </div>
        </section>
        <section class="draw-polkadotParachain" aria-hidden="true">

          <g-image class="i-polkadot" src="~/assets/images/logo-polkadot.png" alt="Polkadot Parachains" />

          <div class="polkadot overflowHide"></div>
          <div class="slot slot-center"></div>

          <div class="overflowHide">
            <div class="slot slot-left"></div>
            <div class="slot slot-right"></div>
          </div>

        </section>
      </section>

      <hr class="animate no-margins" v-in-viewport.once/>


      <section id="strategy" class="animate section__solid section__darkpurple" v-in-viewport.once>

        <div class="layout layout__content">
          <h2>{{$ts('Choose your strategy')}}</h2>

          <section class="grid-3 animate-inside" v-in-viewport.once>
            
            <div>
              <div class="img"><g-image alt="" src="~/assets/images/plo-holder-1.png"/></div>
              <h3>{{$ts('For KSM holders')}}</h3>
              <p class="hyphens">{{$ts('Robonomics PLO may be interesting for stakeholders who are looking for ways to diversify their KSM stake next 48 weeks inside the ecosystem.')}} <g-link to="/xrt/">XRT</g-link> {{$ts('for now is available on Uniswap, Huobi, and in addition on PancakeSwap.')}}</p>
            </div>

            <div>
              <div class="img"><g-image alt="" src="~/assets/images/plo-holder-2.png"/></div>
              <h3>{{$ts('For XRT holders')}}</h3>
              <p class="hyphens">{{$ts('Gain value for your XRT by winning Kusama Slot with Robonomics network great potential for scaling.')}}&nbsp;{{$ts('Take part in our unique staking program: rewarding stakeholders and enabling more zero-weight transactions for IoT devices.')}}</p>
            </div>

            <div>
              <div class="img"><g-image alt="" src="~/assets/images/plo-holder-3.png"/></div>
              <h3>{{$ts('For tech-inspired')}}</h3>
              <p class="hyphens">{{$ts('Robonomics already has complex ecosystem for connecting real world to')}} <g-link to="https:/web3technology-stack.readthedocs.io">{{$ts('Web3 Technology Stack Crowdloan 2')}}</g-link>. {{$ts("It's free, it's opensource, everybody can try it for IoT and Smart services. With Polkadot it can be even more cost-effective.")}}</p>
            </div>

          </section>

          <a href="#a-contribution" class="text-color-red dashed text-big" v-smooth-scroll="{ updateHistory: false, offset: -250 }">Email updates</a>

        </div>
      </section>


      <hr class="animate no-margins" v-in-viewport.once/>

      <section class="animate section__dotted section__solid" v-in-viewport.once>
        <h2 class="layout">{{$ts('Roadmap of the Robonomics parachain')}}</h2>

        <div class="roadmap layout layout__text animate-inside" v-in-viewport.once>
          <h3>{{$ts('Part 1: Establishing core functionality')}}</h3>
          <div class="hyphens">
            <p><b>{{$ts('In 3 months after the Robonomics parachain launch, Robonomics developers are going to activate the core functionally that’s been developing during 2019-2021, and also supplement the network with modules that have proven themselves in the Polkadot and Kusama ecosystems.')}}</b></p>
            <p><b>{{$ts('Genesis state: (0 week)')}}</b> {{$ts('Launch of the starter pack of Robonomics parachain functions with IoT management services and collators reward systems.')}}</p>
            <p><b>{{$ts('Update')}} 1.1</b> {{$ts('Staking and allowing transfers (0 - 1 week). Will allow you to transfer XRT and stake your XRT with a 10% APR for all token holders and 50% for Crowdloan participants.')}}</p>
            <p><b>{{$ts('Update')}} 1.2</b> {{$ts('Treasury and Technical committee (2 - 3 week). Will allow transferring a share of the DAO funds from Ethereum to the parachain. The Technical Committee can produce emergency referenda. These are used for emergency bug fixes or rapid implementation of new but battle-tested features into the runtime.')}}</p>
            <p><b>{{$ts('Update')}} 1.3</b> {{$ts('RWS (4 - 5 week). Will allow using IoT management functions with not only commission payments in XRT but a monthly subscription as well.')}}</p>
            <p><b>{{$ts('Update')}} 1.4</b> {{$ts('Robot-as-a-service (6 - 7 week). Will allow to implement a control process for the provision of automated services and use payments within transactions to launch devices.')}}</p>
            <p><b>{{$ts('Update')}} 1.5</b> {{$ts('XCMP functionality and Robobank (8 - 9 week). The solution is based on the Polkadot XCMP architecture that will allow any parachain to get access to IoT device management with payment in a native token.')}}</p>
            <p><b>{{$ts('Update')}} 1.6</b> {{$ts('Democracy and Remove Sudo (10 - 11 week). Developers won’t have the ability to interfere with the operations of the network without the involvement of the technical committee or voting of parachain native token holders.')}}</p>
          </div>
          <h3>{{$ts('Part 2: Launch services based on Robonomics R&D')}}</h3>
          <div class="hyphens">
            <p><b>{{$ts('2nd part of Robonomics parachain growth in Kusama designated to the launch of services based on previous Robonomics team’s R&D projects.')}}</b></p>
            <p><b>{{$ts('Globally available digital passports of products')}}</b> {{$ts('By supplementing the status of digital twins with information about the produced products, customers will be able to issue digital passports protected against changes and loss of information in the future. This use case is already implemented as a pilot at the enterprise that’s producing drones. The solution used for quality control during packaging with video recording.')}}</p>
            <p><b>{{$ts('Smart leasing of IoT & Robotics')}}</b> {{$ts('We’ll demonstrate the ability to use the Robonomics parachain for leasing an IoT/Robotics device. Using the example of 2 robots controlled by Robonomics parachain in 2 different industries. The first use case - an educational program based on Boston Dynamics SDK, during which developers will learn how to control the famous robot dog - Spot. The second one - an industrial manipulator sold under a leasing agreement in the United States. Both robots will provide customers with automatically generated reports at the end of the user session.')}}</p>
            <p><b>{{$ts('Environmental mitigation services for smart buildings with real carbon credits')}}</b> {{$ts('It will allow customers to automatically collect information about the electricity consumption of the household or apartment building, burn carbon credits, and store a report in the parachain.')}}</p>
            <p><b>{{$ts('Fault-tolerant civil sensors network')}}</b> {{$ts('A complete set of software modules for creating a sensor network in a city or enterprise to track the desired indicators and provide access to them without a central point of failure. Today it is being tested in one of Russian’s industrial cities - Togliatti.')}}</p>
            <p><b>{{$ts('Self-driving cars and drones traffic management solution to avoid route collisions in public areas')}}</b> {{$ts('It’ll allow managing a fleet of drones with publicly monitored access to route changes to public agencies responsible for local security and efficiency of air space and roads')}}.</p>
            <p><b>{{$ts('Ecosystem integration updates')}}</b> {{$ts('We will focus on integrations with other parachains to expand the capabilities of IoT projects that are interested in the Polkadot ecosystem’s features.')}}</p>
          </div>
            <h3>{{$ts('Part 3: Transform into Robonomics Relay Chain')}}</h3>
          <div class="hyphens">
            <p><b>{{$ts('The final task for the 48 weeks of existence in the Kusama network is the transformation of the Robonomics parachain into the Robonomics Relay Chain. This is our vision of the future of Robonomics, as a complete segment of the Polkadot infrastructure specifically prepared for working with IoT devices.')}}</b></p>
          </div>
        </div>≈

      </section>

      <hr class="animate no-margins" v-in-viewport.once/>

      <section class="animate section__darkgray section__solid" v-in-viewport.once>
        <h2 class="layout">{{$ts('Follow latest updates Crowdloan 2')}}</h2>

        <div class="grid-3 animate-inside layout layout__content" v-in-viewport.once>

        <Card orientation="vertical" back="white" :link="$static.metadata.twitter" imageLocal="avatars/twitter.png" imageSize="mid">
          <h3>{{$ts('Robonomics official Twitter Crowdloan 2')}}</h3>
        </Card>

        <Card orientation="vertical" back="white" link="https://twitter.com/EnsRationis" imageLocal="avatars/Sergey-Lonshakov.jpg" imageSize="mid">
          <h3>{{$ts('Software architect Twitter Crowdloan 2')}}</h3>
        </Card>

        <Card orientation="vertical" back="white" :link="$static.metadata.discord" imageLocal="logos/discord.png" imageSize="mid">
          <h3>Robonomics Discord Community</h3>
        </Card>

      </div>

      </section>

    </div>

  </layout>
</template>


<static-query>
query {
  metadata {
    discord,
    twitter
  }
}
</static-query>


<script>

  export default {
    components: {
      MetaInfo: () => import("~/components/MetaInfo.vue"),
      Card: () => import("~/components/TextCard.vue"),
      MovingNumbers: () => import("~/components/decor/MovingNumbers.vue"),
      tip: () => import("~/components/tip.vue"),
      LovelyRoboGirl: () => import("~/components/decor/LovelyRoboGirl.vue"),
      // Subscribtion: () => import("~/components/utils/forms.vue"),
    },


    data () {
      return {
        parachainTab: 1
      }
    },


    methods: {

      infoDetails(e){
        /* This operates with details in crowdloan info - synch open/close */
        if ( window.innerWidth > 880 ) {
          let details = document.querySelectorAll('#info .grid-5 details');

          if(!e.target.parentElement.open) {
            for (let el of details) {
              if(el !== e.target.parentElement){
                el.open = true;
              }
            }
          } else {
            for (let el of details) {
              if(el !== e.target.parentElement){
                el.open = false;
              }
            }
          }
        }
      },

    }
  }
</script>


<style scoped>

  .page {
    --color-polka: #E6007A;
    --color-polka-dark: #9c0053;
  }

  .robogirl {
    max-width: 200px;
    margin: 0 auto;
  }

  #leadership-wrap {
      max-height: 450px;
      overflow: auto;
      margin-top: calc(var(--space)*2);
      margin-bottom: calc(var(--space)*2);
  }
    
  @media screen and (max-width: 700px){
    #leadership {
      table-layout: fixed;
    }

    #leadership td {
      overflow: scroll;
    }
  }

  /* Section Top */
  #info {
    --girl-w: 300px;
    padding-bottom: calc(var(--girl-w) - 10px);
  }

  #info .content, #info {
    position: relative;
    z-index: 1;
  }

  #info-numbers{
    overflow: hidden;
    position: absolute;
    z-index: 0;
    top: 0;
    left: 0;
    right: 0;
    bottom: 0;
  }

  #info .numbers {
    opacity: .4;
  }

  #info-subtitle {
    font-style: italic;
    background-color: var(--color-red);
    display: inline-block;
    padding-left: 0.5rem;
    /* padding-right: 0.5rem; */
  }

  #info-subtitle a {
    display: inline-block;
    background-color: var(--color-green);
    padding-left: 0.5rem;
    padding-right: 0.5rem;
    color: var(--color-light)
  }

  #info h1 { margin-bottom: 0; }

  #info .grid-5{
    font-size: 80%;
  }

  .info-tip {
    font-size: 80%;
    margin-top: calc(var(--space) * 0.5)
  }

  .info-tip a {
    color: var(--color-light)
  }

  #info-girl {
    max-width: var(--girl-w);
    position: absolute;
    bottom: calc((80px + var(--girl-w)) * (-1));
    left: calc(50% - var(--girl-w)/2)
  }

  @media screen and (max-width: 480px) {
    #info {
      --girl-w: 200px;
    }
  }

  @media screen and (max-width: 450px) {
    #info {
      padding-bottom: calc(var(--girl-w) + 20px);
    }
  }
  /* end of Section Top */

  /* Section Contribute */
  .contribution {
    max-width: 760px;
    margin: var(--space) auto;
    text-align: left;
  }

  .contribution span a {
    color: var(--color-light)
  }

  .contribution details[class*='tip'] {
    margin-left: calc(var(--space)*0.5)
  }

  .contribution input[type="checkbox"] {
    float: left
  }

  .contribution > div {
    margin-bottom: var(--space);
  }

  .contribution .checks {
    font-size: 80%;
  }

  .input-signed-right input {
    padding: calc(var(--space) * 0.5)
  }

  .input-signed-right .sign {
    top: 0.8rem
  }

  .button.loading .text {
    display: none;
  }

  .button.loading:before {
      content: "";
      display: inline-block;
      height: 1.2rem;
      width: 1.2rem;
      border-radius: calc(1.2rem/2);
      border-width: 2px 2px 0 0;
      border-style: solid;

      animation: 0.8s Rotate ease-in-out infinite;
    }

  @keyframes Rotate
    {
      0%
        {
          transform:rotate(0deg);
        }
      100%
        {
          transform:rotate(360deg);
        }
    }

    .loader-text, .loader-text-s {
      display: inline-block;
      height: 2rem;
      width: 2rem;
      border-radius: 2rem;
      border-width: 2px 2px 0 0;
      border-style: solid;
      border-color: rgba(255, 255, 255, 0.541);

      animation: 0.8s spin ease-in-out infinite;
    }

    .loader-text-s {
      height: 1rem;
      width: 1rem;
      border-radius: 1rem;
    }
  /* end of Section Contribute */

  /* Section Contribute Step 3 */
  .load-bird {
      position: relative;
      width: 148px;
      height: 180px;
      margin: 0 auto
  }

  .load-bird img { position: absolute; }

  .load-bird img:not(.bird-body) {
      animation-delay: 0.6s;
      animation-duration: 0.8s;
      animation-timing-function: cubic-bezier(0.075, 0.82, 0.165, 1);
      animation-fill-mode: forwards;
  }

  .load-bird .bird-body {
    width: 148px;
    top: 0;
    left: 0;
    z-index: 1;
  }

  .load-bird .bird-tale {
    width: 58px;
    top: 100px;
    left: -35px;
    z-index: 0;

    transform-origin: 0 100%;
  }

  .load-bird .bird-wing-1 {
      width: 47px;
      top: 42px;
      left: 23px;
      z-index: 2;

      transform-origin: 0 0;
    }

   .load-bird .bird-wing-2 {
      width: 67px;
      top: 42px;
      left: 120px;
      z-index: 0;

      transform-origin: 0 0;
    }

    .load-bird .bird-ribbons {
      width: 63px;
      top: 37px;
      left: -8px;
      z-index: 0;

      transform-origin: 100% 50%;
    }

    .load-bird .bird-hair {
        width: 14px;
        top: -10px;
        left: 72px;
        z-index: 0;

        transform-origin: 100% 50%;
      }

    .load-bird .bird-leg {
        width: 37px;
        top: 127px;
        left: 63px;
        z-index: 3;

        transform-origin: 100% 0;
      }


    .crowdloan-step-3.active .in-viewport .bird-tale { animation-name: birdTale; }
    .crowdloan-step-3.active .in-viewport .bird-wing-1 { animation-name: birdWing1; }
    .crowdloan-step-3.active .in-viewport .bird-wing-2 { animation-name: birdWing2; }
    .crowdloan-step-3.active .in-viewport .bird-ribbons { animation-name: birdRibbons; }
    .crowdloan-step-3.active .in-viewport .bird-hair { animation-name: birdHair; }
    .crowdloan-step-3.active .in-viewport .bird-leg { animation-name: birdLeg; }

    .crowdloan-step-3.active .in-viewport .load-bird {
      margin: 0 auto
    }

    .contribution-share {
      margin-top: calc(var(--space)*0.5);
      margin-bottom: var(--space);
      text-align: center;
    }

    .contribution-share a {
        width: 3rem;
    }

     .contribution-share a img {
          display: block;
        }

      .contribution-share a:not(:last-child) {
          margin-right: 0.8rem;
        }
      

      .contribution-share div:not(:last-child) {
        margin-bottom: 0.4rem;
      }
    

    @keyframes birdTale {
      to{
        transform: rotate(25deg) translateX(-20px) translateY(-20px);
      }
    }
    @keyframes birdWing1 {
      to{
        transform: rotate(-50deg) translateX(-25px) translateY(-10px);
      }
    }
    @keyframes birdWing2 {
      to{
        transform: rotate(-50deg) translateX(-25px) translateY(30px);
      }
    }
    @keyframes birdRibbons {
      to{
        transform: rotate(30deg) translateX(-20px);
      }
    }
    @keyframes birdHair {
      to{
        transform: rotate(-30deg);
      }
    }
    @keyframes birdLeg {
      to{
        transform: rotate(-110deg) translateX(10px) translateY(20px);
      }
    }
  /* end of Section Contribute Step 3 */

  /* Section 'Choose your strategy' */
  #strategy .grid-3 { gap: calc(var(--space) * 3) }
  #strategy.section__darkpurple a { color: var(--color-blue-mid) }
  #strategy img { width: 60% }
  @media screen and (max-width: 400px) {
    #strategy img {
      width: 100%
    }
  }
  /* end of Section 'Choose your strategy' */


  /* Section 'Why parachain' */
  .parachain { margin: 0; }
  .parachain section { margin: 0; }

  .parachain .parachains-overview {
      margin-top: calc(var(--space) * 2);
      padding-bottom: 10px;
      border-bottom: 2px dashed #fff;
      position: relative;
      font-size: 90%;
  }

  .parachain h4 { font-size: var(--base-font-size); font-weight: bold; }

  .parachain-intro h2 {
    margin-bottom: calc(var(--space)*2);
  }

  .parachains-overview-line {
    display: grid;
    grid-template-columns: repeat(5, minmax(110px,1fr));
    align-items: start;

    /* scroll */
    width: 100%;
    overflow-x: auto;
    -ms-overflow-style: none;
    scrollbar-width: none;
  }

  .parachains-overview-line::-webkit-scrollbar { display: none; }

  .parachains-overview-line .item {
      opacity: 0.5;
      transform: scale(0.7);
      cursor: pointer;
  }

  .parachains-overview-line .item.active {
    opacity: 1;
    transform: scale(1);
  }

  .parachains-overview-line .item:hover {
      transform: scale(1);
    }

  .parachains-overview-line .item img {
        height: 100px;
        width: auto;
  }

  @media screen and (max-width: 700px) {
    .parachains-overview-line .item img { height: 50px; }
  }

  .parachains-overview-line .item-title {
    font-weight: bold;
    font-family: var(--font-family);
    text-transform: uppercase;
    letter-spacing: 1px;
    font-size: 0.8rem;
    color: #88bcff;
  }

  .parachains-overview-description {
    margin-top: var(--space);
    margin-bottom: var(--space);
  }

  .parachains-overview-description .item {
    opacity: 0;
    display: none;
  }

   .parachains-overview-description .item.active {
        display: block;
        animation: opacity 0.5s linear 0.2s forwards;
      }

    .parachains-overview-description .item h4 {
        margin-bottom: 10px;
      }
    
  
  @keyframes opacity {
    to {
      opacity: 1;
    }
  }

  .draw-polkadotParachain {
    --size-polkadot: 1120px;
    --size-polkadot-logo: 58px;
    --size-slot: 60px;

    background-color: var(--color-purple);
    height: 230px;

    position: relative;
  }

  .draw-polkadotParachain .overflowHide {
      overflow: hidden;
      position: absolute;
      top: 0;
      left: 0;
      right: 0;
      bottom: 0;
    }

  .draw-polkadotParachain .polkadot:after {
        content: "";
        display: block;
        width: var(--size-polkadot);
        height: var(--size-polkadot);
        border-radius: calc(var(--size-polkadot)/1.5);
        background-color: var(--color-polka);
        border: 20px solid var(--color-polka-dark);

        position: absolute;
        top: 65px;
        left: calc(50% - var(--size-polkadot)/2 - 20px);
        z-index: 0;
    }

    .draw-polkadotParachain .i-polkadot {
      position: absolute;
      left: calc(50% - var(--size-polkadot-logo)/2);
      bottom: 28px;
      z-index: 1;

      width: var(--size-polkadot-logo);
    }

    .draw-polkadotParachain .slot {
      position: absolute;
      width: var(--size-slot);
      height: 135px;
      z-index: 0;
    }

    .draw-polkadotParachain .slot:before, .draw-polkadotParachain .slot:after {
      content: "";
      display: block;
    }

    .draw-polkadotParachain .slot:before {
      width: var(--size-slot);
      height: var(--size-slot);
      border-radius: calc(var(--size-slot)/2);
      background-color: var(--color-polka);
    }

    .draw-polkadotParachain .slot:after {
      width: 1px;
      height: 100%;
      border-left: 2px dashed var(--color-polka);

      position: absolute;
      bottom: 0;
      left: calc(50% - 1px);
    }

    .draw-polkadotParachain .slot.slot-center {
      top: calc((-1) * var(--size-slot)/2);
      left: calc(50% - var(--size-slot)/2);
    }

    .draw-polkadotParachain .slot.slot-left, .draw-polkadotParachain .slot.slot-right {
      opacity: 0.5;
    }

    .draw-polkadotParachain .slot.slot-left {
      bottom: 0;
      left: calc(50% - 460px - var(--size-slot)/2);
    }

    .draw-polkadotParachain .slot.slot-right {
      bottom: 0;
      left: calc(50% + 460px - var(--size-slot)/2);
    }

  /* end of Section 'Why parachain' */


  /* Section 'Statistics' */
  #statistics {
    text-align: left;
    padding: 0;
    font-size: 90%;
  }

  #statistics .grid-3 { gap: 0; }
  #statistics .grid-3 > div { padding: var(--space); }
  #statistics .grid-3 > div:nth-child(2) { background-color: #141414; }
  #statistics .grid-3 > div:nth-child(3) { background-color: #000; }
  /* end of Section 'Statistics' */

</style>

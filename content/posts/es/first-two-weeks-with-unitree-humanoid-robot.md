---
title: 'Las Primeras Dos Semanas Trabajando con el Robot Humanoide Unitree G1'
date: 2024-12-27
published: true
locale: 'es'
tags: ['Robótica', 'ROS 2']
cover_image: ../images/first-two-weeks-with-unitree-humanoid-robot/cover.webp
description: "Han pasado dos semanas desde que el robot humanoide Unitree G1 llegó al laboratorio de Robonomics. Un equipo de al menos cinco ingenieros con maestrías en robótica se puso inmediatamente a trabajar estudiando y programando el nuevo dispositivo. ¡Queremos compartir las primeras noticias del campo: impresiones, hallazgos y desafíos en el camino hacia, esperamos, una revolución humanoide!"
abstract: "Han pasado dos semanas desde que el robot humanoide Unitree G1 llegó al laboratorio de Robonomics. Un equipo de al menos cinco ingenieros con maestrías en robótica se puso inmediatamente a trabajar estudiando y programando el nuevo dispositivo. ¡Queremos compartir las primeras noticias del campo: impresiones, hallazgos y desafíos en el camino hacia, esperamos, una revolución humanoide!"
---

## TL;DR

- Conexión exitosa con la unidad de desarrollo / PC2 (ver diagramas abajo).
- Configuración de una conexión remota a través de **SSH** mediante **Zerotier** y **Yggdrasil**.
- Estudio del sistema basado en Linux a bordo del humanoide, realización de tareas estándar de DevOps.
- Conocimiento de la biblioteca **Python SDK** desdedesarrolladores (¡incluso corregimos un error crítico!): ahora podemos controlar el robot desde scripts: caminar, sentarse, levantarse y amortiguar.
- Construimos **paquetes ROS 2**, conectados a temas, lanzamos varios ejemplos, pero se requiere realizar pruebas adicionales.

<rb-image zoom src="./images/first-two-weeks-with-unitree-humanoid-robot/image-schemes.webp" alt="Transmisión de datos del robot humanoide Unitree" />

## Notas del Campo

**Sobre el SDK de Python:**

- Utilizamos un entorno virtual (**venv**) en **Python 3.10** — el SDK no funciona con otras versiones.
- Trabajamos a través de la interfaz **eth0** desde la unidad de desarrollo.
- Aunque **CycloneDDS** estaba preinstalado, se reconstruyó manualmente sin conflictos.
- Para ejecutar scripts, es necesario establecer una variable de entorno (se recomienda agregarla a `.bashrc`). **Importante:** especificar la ruta completa entre comillas simples:

<rb-code>

```
export CYCLONEDDS_HOME='/home/unitree/cyclonedds/install'
```
</rb-code>

- Los scripts no funcionan en el modo de depuración del robot, aunque según la documentación deberían.
- Para corregir el SDK y hacer que el robot se mueva, agregamos la línea `self.Start()` a la función `Move()` del archivo **g1_loco_client.py**.

**Sobre ROS 2**

- Construimos paquetes del repositorio **unitree_ros2**, incluido el soporte de **CycloneDDS**.- Obtener los archivos del paquete construido para agregarlos al entorno de ROS 2.
- Entre los ejemplos:
  - Se recibieron con éxito los estados del controlador.
  - Los ejemplos relacionados con los estados de movimiento no funcionaron (los temas están vacíos).
- Los paquetes se pueden utilizar para crear sus propios nodos de ROS (ya sea en Python o C++).

<rb-grid :columns="2" textAlign="center" align="end">
  <rb-grid-element>
    <rb-image zoom src="./images/first-two-weeks-with-unitree-humanoid-robot/first-entering.webp" alt="Primer ingreso del robot humanoide Unitree" />
  </rb-grid-element>
  <rb-grid-element>
    <rb-image zoom src="./images/first-two-weeks-with-unitree-humanoid-robot/cyclonedds-error.webp" alt="Error de CycloneDDS del robot humanoide Unitree" />
  </rb-grid-element>
</rb-grid>

## Plan de Tareas

1. **Verificar la posibilidad de suministro de energía desde el cable.** Tal vez esta función ya exista, necesitamos revisar la documentación eléctrica o adquirir un cable adecuado.
2. **Comprender el modo de depuración para el SDK.** La documentación indica que funciona, pero en la práctica no lo hace.
3. **Falta de ejemplos avanzados.** Los repositorios se limitan a acciones básicas (sentarse, levantarse, control de motores). Para CES 2025, necesitamos adaptar soluciones simples listas o desarrollar algoritmos de movimiento de bajo nivel.4. **Elección de tecnología:**
  - Todo el proceso se puede implementar en **Python**, incluida la integración con Robonomics.
  - Sin embargo, es preferible utilizar **ROS 2** por su estructura y escalabilidad.
5. **Estudiar métodos de aprendizaje por refuerzo** para su posible uso en el control de robots.

## Enlaces útiles

- Repositorio principal: [https://github.com/unitreerobotics](https://github.com/unitreerobotics)   
- SDK de Python: [https://github.com/unitreerobotics/unitree_sdk2_python](https://github.com/unitreerobotics/unitree_sdk2_python)   
- Paquetes de ROS 2: [https://github.com/unitreerobotics/unitree_ros2](https://github.com/unitreerobotics/unitree_ros2)  
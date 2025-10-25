---
layout: post
title: "Virtualización de una tarjeta de video NVIDIA Geforce GTX680 en Openstack"
categories: openstack
author: "Jose A. Martinez"
---

La integración de aceleradores gráficos en entornos de cómputo virtualizado se ha convertido en una práctica esencial para mejorar el rendimiento en tareas intensivas como el procesamiento paralelo, la renderización 3D o el entrenamiento de modelos de inteligencia artificial. En este contexto, la capacidad de un entorno OpenStack para aprovechar una GPU física mediante PCI passthrough representa una de las configuraciones más potentes y versátiles disponibles para entornos de virtualización de alto rendimiento (HPC).

En este [manual][Enlace] exploraremos el proceso de instalación y configuración de una tarjeta de video Nvidia GeForce GTX 680 en un nodo de cómputo de OpenStack, con el objetivo de habilitar su uso directo por máquinas virtuales. Aunque la GTX 680 no pertenece a la línea profesional de Nvidia, su arquitectura Kepler y soporte para CUDA la convierten en una excelente opción experimental o de laboratorio para probar las capacidades de GPU passthrough en OpenStack.

El procedimiento abordará desde la detección del dispositivo PCI y la configuración de los módulos del kernel necesarios para su aislamiento, hasta la definición de los parámetros en nova.conf y la asignación de la GPU a las instancias virtuales. También revisaremos consideraciones importantes sobre compatibilidad de hardware, BIOS, IOMMU y drivers Nvidia. Al final del proceso, el resultado será un entorno OpenStack capaz de ofrecer instancias virtuales con acceso directo a la GPU física, permitiendo ejecutar cargas de trabajo aceleradas con el rendimiento casi nativo del hardware.

👉 [Virtualización de una tarjeta de video NVIDIA Geforce GTX680 en Openstack][Enlace]

[Enlace]: http://hpcjmart.github.io/gtx680

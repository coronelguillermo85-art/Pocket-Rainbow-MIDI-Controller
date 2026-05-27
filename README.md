
<img src="https://img.shields.io/badge/Project-Sensitive_Lab-blueviolet?style=for-the-badge" alt="Sensitive Lab"> <img src="https://img.shields.io/badge/License-MIT-yellow?style=for-the-badge" alt="MIT License">

# 🎛️ Pocket Rainbow Midi Controller (Hardware Open-Source)

Este repositorio contiene la documentación técnica, el diseño de hardware y el firmware para el **Pocket Rainbow Midi Controller**, un controlador MIDI dinámico, ultra compacto y personalizado. El dispositivo está construido sobre un microcontrolador **ESP32-S3 (Módulo N16R8)** y cuenta con una matriz física de 16 pulsadores de alta respuesta, diseñada específicamente para la ejecución de instrumentos virtuales y sintetizadores en tiempo real.

> 🌈 *Nota del Diseñador:* Bautizado como "Pocket Rainbow" debido a la estética de su ensamble interno; el ordenado cableado plano de colores utilizado para rutear las señales evoca un arcoíris emergiendo directamente desde el corazón del circuito.

---

## 📸 Ingeniería de Hardware & Ensamble

El desarrollo físico se diseñó bajo una filosofía purista de hardware libre (*logic maker*), priorizando la robustez mecánica, el tamaño portátil y un ruteo limpio de señales:

* **Arquitectura de Conexión:** Distribución de pines optimizada sobre placa perforada de alta densidad mediante un sistema de cableado plano tipo cinta arcoíris para mitigar ruidos electromagnéticos y mantener la prolijidad visual.
* **Montaje del Microcontrolador:** Integración del ESP32-S3 sobreelevado mediante tiras de headers hembra para facilitar la refrigeración, el mantenimiento del módulo y optimizar el espacio inferior de la placa para las soldaduras de la matriz.
* **Matriz de Pulsadores:** Configuración de 16 botones táctiles cableados en filas y columnas, permitiendo escanear múltiples entradas físicas utilizando una cantidad mínima de pines GPIO esenciales del microcontrolador.

---

## 🛠️ Especificaciones Técnicas

* **Cerebro Central:** ESP32-S3 de alta performance (16MB Flash, 8MB PSRAM).
* **Protocolos Soportados:** * **USB-MIDI Nativo:** Reconocimiento automático como dispositivo *Plug & Play* (clase compatible) sin necesidad de drivers en Windows, macOS o Linux.
  * **BLE MIDI (Bluetooth Low Energy):** Conectividad inalámbrica de ultra baja latencia para setups móviles o escenarios en vivo.
* **Procesamiento de Señal (Firmware):** Algoritmo de multiplexación por software con lógica de *software debounce* optimizada para evitar falsas pulsaciones y garantizar que cada nota se active al instante.

---

## 🚀 Filosofía del Proyecto

> *"No hay nada mejor para un músico o luthier electrónico que tocar con los instrumentos y herramientas que uno mismo diseña, suelda y programa desde los cimientos."*

Este módulo portátil está pensado de forma transversal: puede funcionar como un secuenciador de pasos, un lanzador de muestras (*sampler pad*) o un panel interactivo de control de comandos (CC) para performances de música electrónica, futurepop o sintetizadores modulares.

---
<img width="1204" height="1600" alt="WhatsApp Image 2026-05-26 at 10 27 03 PM" src="https://github.com/user-attachments/assets/b294c636-18c7-411e-8b45-74a78b43f3ee" />


---
🚀 *Proyecto en constante optimización. Desarrollado con soldadura de precisión, código limpio y pasión por el hardware libre.*

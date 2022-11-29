# Diseño e implementación del encapsulado para un prototipo de estimulador del nervio vago, y de un nervio vago artificial, como plataforma de pruebas para el estimulador

<p align="center">
<img src="https://github.com/ionas-UVG/Tesis-2022-Nervio-Vago-Artificial/blob/5153043706a7ae2c09a8a88e634a6104756698e3/Documentos/Imagenes/GIF/neuron.gif" height="150"> <img src="https://github.com/ionas-UVG/Tesis-2022-Nervio-Vago-Artificial/blob/e79cc0adab2fa9ac0317886fba2164efc780ccc1/Documentos/Imagenes/GIF/action-potential-graphics.gif" height="150"><img src="https://github.com/ionas-UVG/Tesis-2022-Nervio-Vago-Artificial/blob/2e7fbe03dd19fab017b71f1059ad863009ae48de/Documentos/Imagenes/GIF/vns%20therapy.gif" height="150"><img src="https://github.com/ionas-UVG/Tesis-2022-Nervio-Vago-Artificial/blob/e79cc0adab2fa9ac0317886fba2164efc780ccc1/Documentos/Imagenes/GIF/pcb.gif" height="150">
 </p>
 
## Visión General
Este proyecto se centró en el desarrollo de un primer prototipo de Nervio Vago Artificial como una plataforma de pruebas para evaluar los parámetros elécricos de la señal de salida del estimulador del nervio vago desarrollado en fases anteriores. En este repositorio se almacenan los avances obtenidos en esta primera fase.

## Objetivos
Los objetivos para este proyecto fueron:
* Seleccionar el modelo adecuado para la implementación en físico del nervio vago artificial.  
* Desarrollar circuitos electrónicos impresos para la plataforma de pruebas del estimulador del nervio vago.  
* Diseñar e implementar un primer prototipo de encapsulado para el estimulador del nervio vago desarrollado en la fase anterior.

## Unidad de Neurona FitzHugh-Nagumo
Para la construcción del Nervio Vago Artificial se seleccionó el modelo neuronal de FitzHugh-Nagumo. Este modelo cuenta con tres etapas. La etapa pasiva conformada por la resistencia y capacitancia de la membrana celular, la etapa de Sodio (repolarización) y la etapa de Potasio (polarización).
 
 ### Simulaciones
 
 Para las simulaciones se utilizó la herramienta de simulación LTspice. A continuación, se listan las simulaciones realizadas:
 
 * **Unidad de Neurona FitzHugh-Nagumo:** Se simularon cada una de las etapas que conforman el modelo neuronal seleccionado y realizaron pruebas con señales de distintas amplitudes y frecuencias.
 * **Axón Módular:** Se definieron como componentes la unidad de neurona FitzHugh-Nagumo y el módulo de acondicionamiento y se utilizaron para la construcción de un axón de neurona de 5 segmentos, con el fin de observar el comportamiento del estímulo aplicado conforme atraviesa el axón. 
 * **Unidad de Alimentación:** Se realizaron pruebas con el módulo de alimentación construido. Este se construyó a partir de un NE555 que genera un voltaje negativo de 12V a partir de la alimentación proveída por un transformador de 12V.

<p align="center">
<img src="https://github.com/ionas-UVG/Tesis-2022-Nervio-Vago-Artificial/blob/b51f45b2c370843a8341eafaf512505e302ee61d/Documentos/Imagenes/ltspice-sim.png" width="700"> 
</p>

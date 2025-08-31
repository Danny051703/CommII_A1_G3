
# Práctica 1. Reconocimiento de equipos, GNU Radio, Mediciones de potencia y frecuencia

### Integrantes
- **Danny Carolina Sierra Téllez** - 2220409
- **Duban Andretti Gutierréz León** - 2220

Escuela de Ingenierías Eléctrica, Electrónica y de Telecomunicaciones  
Universidad Industrial de Santander

### Fecha
31 de agosto de 2025

---
## Contenido

### Resumen
En esta práctica se implementaron conceptos de radio definida por software (SDR) utilizando la plataforma GNU Radio. El trabajo incluyó la familiarización con el manejo de repositorios en GitHub desde un entorno de programación colaborativo, integrando la terminal local con la nube para simular un trabajo similar al de la industria. Se desarrollaron bloques de programación en Python para implementar funciones como un acumulador, diferenciador y otros operadores estadísticos sobre señales en el dominio del tiempo. Estas implementaciones permitieron fortalecer la comprensión de los sistemas de comunicaciones digitales en tiempo real y evidenciaron la flexibilidad de GNU Radio para el diseño, análisis y evaluación de sistemas de procesamiento de señales.


### Introducción
En comunicaciones es clave el procesamiento y análisis de las señales para garantizar un buen proceso de transmisión y recepción de mensajes. Dentro de las medidas que están directamente relacionadas a estas, se destacan: la potencia, el piso de ruido y el ancho de banda; escenciales para buscar mejoras y evaluar los procesos de los sistemas de comunicación. Ahora bien, en la asignatura se hace uso de la herramienta de GNU Radio, así como de otros equipos de laboratorio como osciloscopio, analizador de espectros, antenas, radio entre otros; los cuales, permiten estudiar la relación de las medidas anteriormente mencionadas en el cambio de diferentes condiciones a señales.

## Declaración de Originalidad y Responsabilidad
Los autores de este informe certifican que el contenido aquí presentado es original y ha sido elaborado de manera independiente. Se han utilizado fuentes externas únicamente como referencia y han sido debidamente citadas.

Uso de IA: Se utilizó para reformular ciertas secciones del texto, verificar gramática, y optimizar la redacción general. Sin embargo, el contenido técnico, análisis y las conclusiones del informe, fueron desarrollados por los autores.

---
## Contenido

## **Objetivo General**

Familiarizarse con el uso de herramientas de software definido por radio (SDR) como GNU Radio, junto con equipos de medición como el USRP 2920, el osciloscopio R&S RTB2004 y el analizador de espectros R&S FPC1000. Aprender a medir y analizar parámetros clave en comunicaciones, como potencia, ancho de banda, relación señal a ruido (SNR) y piso de ruido.

---

### Procedimiento

## **Materiales y Equipos**
- **USRP 2920**: Radio definido por software.
- **Osciloscopio R&S RTB2004**: Para visualización de señales en el dominio del tiempo y frecuencia.
- **Analizador de Espectros R&S FPC1000**: Para mediciones en el dominio de la frecuencia.
- **Computador con GNU Radio**: Para simulación y generación de señales usando el USRP 2920.
- **Cables y conectores**: Para interconexión de equipos.

---

## **Actividad 1: Revisión de Especificaciones de los Equipos**

### **Objetivo**
Familiarizarse con las especificaciones técnicas de los equipos de laboratorio y entender cómo configurarlos para realizar mediciones.

### **Procedimiento**
1. Se revisaron los manuales sobre cada uno de los equipos usados durante el desarrollo de las clases de laboratorio, con el fin de identificar especificaciones relevantes así como modo de uso, herramientas y controles de los mismos.
  
2. **Evidencia  y especificaciones Relevantes**:
   *USRP 2920*
      - Rango de frecuencia:  50MGz a 2.2GHz
      - Ganancia configurable: 0 a 31.5dB pasos de 0.5dB
      - Ancho de banda: 20M a 40MHz
      - Resolución de frecuencia: <1kHz
      - Potencia máxima de salida: 50m a 100mW
        

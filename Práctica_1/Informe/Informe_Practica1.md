
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
La Radio Definida por Software (SDR) cumple un papel fundamental en las telecomunicaciones modernas gracias a su flexibilidad y adaptabilidad. Esta tecnología permite que una misma plataforma soporte múltiples estándares y pueda soportar una amplia variedad de señales sólo con usar una computadora y software especializado, reconfigurando tareas relacionadas con la transmisión y recepción de señales de radiofrecuencia.
En el marco de la práctica, se implementaron bloques en Python dentro de GNU Radio para simular funciones clásicas tales como un acumulador, diferenciador y operadores estadísticos de las señales en el tiempo como: la media, media cuadrática, valor RMS, densidad de potencia espectral y desviación estándar. Dichos bloques ofrecen una herramienta útil para analizar el comportamiento de señales digitales en tiempo real y constituyen una base para el desarrollo de aplicaciones más avanzadas en escenarios de la vida real en telecomunicaciones.


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
        

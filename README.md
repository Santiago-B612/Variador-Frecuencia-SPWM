# Variador de Frecuencia para Motores AC (Técnica SPWM)

## 📝 Descripción
Este proyecto consiste en el diseño y análisis de un variador de frecuencia capaz de controlar la velocidad de un motor de inducción mediante la modulación por ancho de pulso senoidal (SPWM). El sistema realiza una conversión completa de energía desde una red AC monofásica hacia una salida AC con frecuencia variable.

## 🛠️ Especificaciones Técnicas
- **Topología:** Inversor de puente completo (Full Bridge).
- **Técnica de Modulación:** SPWM (Sinusoidal Pulse Width Modulation).
- **Etapa de Potencia:** MOSFETs IRF840 con Drivers IR2112.
- **Frecuencia de Conmutación:** [Insertar Hz aquí, ej: 2kHz].
- **Filtrado:** Filtro pasabajas LC de segundo orden para reconstrucción de onda.

## 📐 Bloques del Sistema
1. **Conversión AC-DC:** Rectificación de onda completa (1N4004) y filtrado capacitivo (Bus DC de 166V).
2. **Generación de Control:** Comparación de señal portadora (triangular) y moduladora (senoidal) mediante LM324.
3. **Drivers de Disparo:** Aislamiento y control de compuerta (Gate) para el puente H.
4. **Etapa de Salida:** Filtrado LC y conexión a motor trifásico adaptado.

## 🚀 Resultados
- Reducción de distorsión armónica total (THD).
- Control efectivo de la relación Voltaje/Frecuencia (V/f).

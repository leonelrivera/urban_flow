# Proyecto Urban Flow - Sprint 1
## Objetivo: Análisis y limpieza de datos de radares.
Contexto: Localidad de Vaalserberg, sistema de radares urbanos.

## Conclusiones del Sprint 1
El análisis del dataset Urban Flow ha permitido identificar que el sistema de
registro original presentaba una degradación significativa en la precisión
temporal, evidenciada por el alto porcentaje de registros que requirieron
normalización (fechas de 1932 y horas 00:00).

A pesar de estas limitaciones, la limpieza y el procesamiento con Pandas
permitieron recuperar la trazabilidad de las infracciones. Se determinó que
existe una reincidencia crítica en un grupo reducido de patentes y que los
excesos de velocidad reales superan con frecuencia el margen de tolerancia
del 5%, lo que subraya la importancia de este proceso de depuración para
la gestión del tráfico en Vaalserberg.
# Conclusión: Relación entre Imágenes y Datos (Sprint 2)

El desarrollo de este Trabajo Práctico demuestra cómo el **Procesamiento Digital de Imágenes (PDI)** y el **Reconocimiento Óptico de Caracteres (OCR)** actúan como un puente indispensable para transformar datos no estructurados (imágenes de cámaras de tráfico) en registros estructurados aptos para la toma de decisiones.

### Puntos Clave de la Relación:
1. **La Calidad del Dato Visual Impacta en el Negocio:** La tasa de éxito del OCR (*EasyOCR*) está directamente condicionada por la etapa de PDI. Sin el filtrado morfológico, suavizado Gaussiano y detección de bordes (Canny), el ruido del entorno (luces, asfalto, tornillos) genera lecturas erróneas. El procesamiento espacial purifica la imagen para aislar la geometría de la patente.
2. **Cruce de Universos de Datos:** Logramos asociar una única entidad visual (el vehículo fotografiado) con su histórico en el dataset estructurado del Sprint 1 (`speeding_fines.csv`). Esto permite identificar patrones críticos como la **reincidencia** (un mismo auto con múltiples infracciones pendientes).
3. **Consistencia e Integridad Automatizada:** Las métricas integradas exponen la brecha entre la detección teórica del radar y la evidencia física. Un sistema de auditoría real exige que el 100% de las deudas monetarias activas cuenten con su respaldo en formato `path` de imagen y un `ratio` de confianza matemática superior al 80%, blindando el sistema contra falsos positivos y reclamos legales.

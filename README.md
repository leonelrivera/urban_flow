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

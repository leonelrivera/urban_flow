# Changelog

## [2026-04-19]
- Inicialización del proyecto.

## [2026-04-19] - Ejercicio 02
- Implementación de descarga automatizada de datos.
- Análisis exploratorio inicial (head, info, nulls).

## [2026-04-19] - Ejercicio 03
- Normalización de fechas (1932-01-01) y horas (00:00).
- Limpieza de strings en ubicaciones y patentes.
- Eliminación de nulos y outliers de velocidad.
- Creación de columnas de cálculo de exceso (real y margen 5%).
- Guardado de dataset procesado en data/interim.

## [2026-04-25] - Ejercicio 04
- Implementación de la clase FineAnalyzer para encapsulamiento de lógica.
- Creación de métodos de ranking para patentes y horarios (Top 5).
- Cálculo de métricas promedio de exceso de velocidad.
- Agrupación de multas por ubicación geográfica.

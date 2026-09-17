# TFB · CPD sostenibles en la Península Ibérica

Este repositorio contiene el desarrollo técnico de nuestro Trabajo Final de Bàtxelor en Ciencia de Datos:

**Modelo geoespacial multivariante y multicriterio para evaluar zonas potencialmente adecuadas para la instalación de centros de procesamiento de datos sostenibles en la Península Ibérica.**

El objetivo es comparar la idoneidad territorial de las regiones analizadas a partir de información pública y reproducible. Para ello trabajamos con datos climáticos, solares, territoriales, ambientales, eléctricos, logísticos, digitales, demográficos y de estrés hídrico.

El modelo sirve como apoyo para comparar territorios. No pretende decidir una parcela concreta ni determinar de forma automática dónde debe instalarse un centro de datos.

## Ámbito de estudio

Trabajamos con **22 regiones NUTS 2 de España peninsular y Portugal continental**.

También incluimos **Andorra como unidad nacional complementaria**, aunque no participa en el ranking final del IIT-CPD por falta de datos comparables en algunas dimensiones.

No se incluyen los territorios insulares.

## Notebooks

El proyecto se organiza en **16 notebooks de Python**, siguiendo el orden real de trabajo.

| Notebook | Contenido principal |
| --- | --- |
| 01 · ERA5-Land | Datos climáticos 2024–2025 |
| 02 · CORINE Land Cover | Cobertura y compatibilidad del suelo |
| 03 · OSM / Geofabrik | Logística y accesibilidad |
| 04 · PVGIS | Potencial solar fotovoltaico |
| 05 · Medio ambiente | Espacios protegidos |
| 06 · Infraestructura eléctrica | Líneas eléctricas y subestaciones |
| 07 · Conectividad digital | Infraestructura de telecomunicaciones |
| 08 · Demografía y capital humano | Población, empleo y formación |
| 09 · Geometrías territoriales | Base geográfica común |
| 10 · Dataset maestro | Integración territorial |
| 11 · Auditoría y EDA | Control de calidad y análisis exploratorio |
| 12 · Matriz multivariante | Selección y preparación de variables |
| 13 · Isolation Forest | Detección exploratoria de singularidades |
| 14 · PCA | Análisis de componentes principales |
| 15 · K-Means | Perfiles territoriales |
| 16 · IIT-CPD y Pareto | Modelo multicriterio, sensibilidad y Pareto |

Los Notebooks 01–09 preparan las distintas fuentes de datos. El Notebook 10 las integra en un dataset maestro de **23 territorios y 113 columnas**, con **74 variables analíticas**.

Después del EDA y la selección de variables trabajamos con una matriz de **22 territorios y 21 variables**.

Utilizamos Isolation Forest, PCA y K-Means para entender mejor la estructura de los datos y los perfiles territoriales. No los utilizamos para asignar directamente los pesos del índice.

## IIT-CPD

El Notebook 16 construye el **Índice de Idoneidad Territorial para Centros de Procesamiento de Datos (IIT-CPD)**.

El índice utiliza **16 variables activas agrupadas en ocho dimensiones**: clima, energía solar, territorio, medio ambiente, infraestructura eléctrica, logística y conectividad digital, capital humano y estrés hídrico.

Comparamos cuatro escenarios:

- Equilibrado
- Energético
- Ambiental
- Tecnológico

También realizamos pruebas de sensibilidad y un análisis de Pareto para comprobar la estabilidad de los resultados y los compromisos entre dimensiones.

## Análisis multivariante

Después de seleccionar las 21 variables:

- Isolation Forest identifica territorios con comportamientos singulares.
- El PCA utiliza 19 variables y conserva tres componentes, que explican el **74,54 % de la varianza**.
- K-Means utiliza estos componentes para obtener **seis perfiles territoriales**.

Estos análisis sirven como apoyo para interpretar los resultados y no modifican directamente el cálculo del IIT-CPD.

## Datos

Las fuentes no pertenecen todas al mismo año.

ERA5-Land utiliza el periodo **2024–2025**. Para el resto de los datos usamos la información más reciente disponible que permite mantener una cobertura comparable entre territorios.

Por eso, el dataset final reúne información de distintos años y no lo utilizamos como una serie temporal.

## Power BI

Power BI utiliza las salidas obtenidas en Python para consultar de forma conjunta el IIT-CPD, los perfiles territoriales y el resto de resultados del análisis.

Realizamos los cálculos del modelo en los notebooks y no en Power BI.

## Reproducibilidad

En GitHub dejamos los notebooks, la documentación, los diagramas y los archivos necesarios para seguir el trabajo.

Los datos y resultados de mayor tamaño los guardamos aparte y dejamos indicada su procedencia y cómo los hemos obtenido.

## Autores

**Antonio Eloy Martínez Jiménez**  
**Alberto Sanz Viñuela**

Bàtxelor en Ciencia de Datos  
Universitat Carlemany

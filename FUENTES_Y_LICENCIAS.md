# Fuentes y licencias

Este documento reúne las fuentes utilizadas en el TFB **Localización sostenible de centros de datos** y las condiciones que debemos tener en cuenta al publicar sus resultados.

En algunos notebooks reutilizamos archivos disponibles en Kaggle Input. Kaggle es en esos casos el lugar desde el que recuperamos el archivo, pero no sustituye a la fuente original.

Los datos tampoco corresponden todos al mismo año. El proyecto combina la información reciente que hemos podido obtener de forma comparable para cada dimensión.

Última revisión: **24 de agosto de 2026**.

## Fuentes utilizadas

| Notebook | Fuente | Uso en el proyecto | Licencia o condición principal |
| --- | --- | --- | --- |
| 01 | [ERA5-Land · Copernicus Climate Data Store](https://cds.climate.copernicus.eu/datasets/reanalysis-era5-land) | Variables climáticas 2024–2025 | CC BY 4.0. DOI: [10.24381/cds.e2161bac](https://doi.org/10.24381/cds.e2161bac) |
| 02 | [CORINE Land Cover 2018](https://land.copernicus.eu/en/products/corine-land-cover/clc2018) | Cobertura y compatibilidad del suelo | Reutilización según política de Copernicus. DOI: [10.2909/960998c1-1870-4e82-8051-6485205ebbac](https://doi.org/10.2909/960998c1-1870-4e82-8051-6485205ebbac) |
| 03, 06 y 07 | [OpenStreetMap](https://www.openstreetmap.org/copyright) | Carreteras, núcleos de población, infraestructura eléctrica y elementos de telecomunicaciones | ODbL 1.0. Debe mantenerse la atribución a OpenStreetMap y sus colaboradores |
| 03 | [Geofabrik](https://download.geofabrik.de/) | Extractos de OpenStreetMap para España, Portugal y Andorra | Se mantienen las condiciones de OSM/ODbL |
| 06 y 07 | [Overpass API](https://overpass-api.de/) | Consultas específicas sobre elementos de OpenStreetMap | Los datos recuperados mantienen la licencia de OSM |
| 04 | [PVGIS · European Commission JRC](https://joint-research-centre.ec.europa.eu/pvgis-online-tool_en) | Potencial solar fotovoltaico | Reutilización del contenido de la Comisión Europea; indicamos PVGIS/JRC y los cálculos realizados por nosotros |
| 05 | [EEA · Natura 2000](https://bio.discomap.eea.europa.eu/arcgis/rest/services/ProtectedSites/Natura2000Sites/MapServer) | Espacios protegidos de España y Portugal | Reutilización según las condiciones de la European Environment Agency |
| 05 | [EEA · Emerald Network](https://bio.discomap.eea.europa.eu/arcgis/rest/services/ProtectedSites/EmeraldSites/MapServer) | Espacios protegidos de Andorra | Reutilización según las condiciones de la EEA |
| 07 | [PeeringDB](https://www.peeringdb.com/apidocs/) | Facilities y puntos de intercambio de Internet | Uso sujeto a su Acceptable Use Policy. No redistribuimos la base completa |
| 07 | [RIPE Atlas](https://atlas.ripe.net/api/v2/probes/) | Probes activos como indicador complementario de conectividad | Uso sujeto a las condiciones de RIPE NCC |
| 08 | [Eurostat](https://ec.europa.eu/eurostat/web/user-guides/data-browser/api-data-access/api-introduction) | Población, densidad, desempleo y formación terciaria de España y Portugal | Reutilización permitida con reconocimiento de la fuente, salvo excepciones específicas |
| 08 | [World Bank Indicators API](https://api.worldbank.org/v2/) | Indicadores nacionales complementarios de Andorra | Condiciones de reutilización del Banco Mundial; normalmente CC BY 4.0 salvo indicación específica |
| 09 | [GISCO / Eurostat](https://ec.europa.eu/eurostat/web/gisco/geodata/statistical-units) | Geometrías NUTS 2024 | Para los límites administrativos mantenemos `© EuroGeographics for the administrative boundaries` |
| 09 | [Natural Earth](https://www.naturalearthdata.com/about/terms-of-use/) | Geometría complementaria de Andorra y límites auxiliares | Dominio público |
| 10 | [EEA · WEI+](https://www.eea.europa.eu/en/datahub/datahubitem-view/5a980253-9e62-4004-830e-ae7a985237b9) | Estrés hídrico, periodo 2019–2023 | Condiciones de reutilización de la EEA |
| 10 | International Monetary Fund | Tasa de desempleo de Andorra para 2024 | IMF Country Report No. 26/88. DOI: [10.5089/9798229045056.002](https://doi.org/10.5089/9798229045056.002) |

## Algunas consideraciones

En OpenStreetMap utilizamos la atribución:

`© OpenStreetMap contributors. Datos disponibles bajo ODbL 1.0.`

Para ERA5-Land identificamos Copernicus Climate Change Service y dejamos claro que los datos han sido procesados por los autores.

En los resultados de PVGIS indicamos **European Commission, Joint Research Centre (JRC), PVGIS 5.3** y diferenciamos los datos de los cálculos realizados en el TFB.

Las coordenadas publicadas por RIPE Atlas están desplazadas deliberadamente por privacidad. Las utilizamos para indicadores territoriales y no intentamos reconstruir la localización exacta de los probes.
No redistribuimos las bases originales completas de terceros cuando no hace falta. El repositorio contiene código, documentación y resultados derivados.

## Fuentes utilizadas como contraste

En el Notebook 06 consultamos también **Redeia, REN, ENTSO-E y FEDA** como referencias de contexto.

No utilizamos datos de estas fuentes para calcular los indicadores eléctricos del modelo. Las variables eléctricas incorporadas al análisis proceden de OpenStreetMap.

## Notebooks 11–16

Los Notebooks 11–16 no añaden nuevas fuentes primarias.

Los Notebooks 11–16 trabajan con las salidas anteriores para realizar la auditoría y el EDA, preparar la matriz multivariante, aplicar Isolation Forest, PCA y K-Means y construir el IIT-CPD y el análisis de Pareto.

## Licencia del repositorio

El repositorio no contiene un archivo `LICENSE`.

Por tanto, no asumimos una autorización general para copiar, modificar o redistribuir el código. Si más adelante añadimos una licencia propia, seguiremos respetando las condiciones de las fuentes externas que hemos utilizado.

Mantenemos las atribuciones y restricciones que indica cada proveedor, aunque añadamos una licencia al repositorio.

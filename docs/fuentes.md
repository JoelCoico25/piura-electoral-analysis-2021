# Fuentes de datos

Este proyecto integra datos públicos de la ONPE, el INEI y el PNUD para analizar la participación electoral distrital en Piura durante las dos vueltas presidenciales de 2021.

**Nota de trazabilidad:** los enlaces siguientes corresponden a publicaciones oficiales pertinentes que fueron localizadas y comprobadas como páginas institucionales. **No se ha contrastado de manera exhaustiva que cada archivo local utilizado en Power BI coincida exactamente con la versión o recurso descargable actualmente publicado**. En particular, quedan pendientes de contrastar las versiones de los anexos de pobreza, la tabla de IDH y el catálogo UBIGEO. Los enlaces se ofrecen como referencias oficiales para consultar y recuperar los datos, no como certificación de identidad archivo por archivo.

## Referencias oficiales

| Institución | Datos utilizados | Año | Publicación oficial | Estado de correspondencia |
|---|---|---|---|---|
| ONPE | Resultados por mesa, primera vuelta presidencial | 2021 | [Resultados por mesa — Primera vuelta](https://www.datosabiertos.gob.pe/dataset/resultados-por-mesa-de-las-elecciones-presidenciales-2021-primera-vuelta-oficina-nacional-de) | El recurso publicado incluye `Resultados_1ra_vuelta_Version_PCM.csv`; falta contraste integral del archivo local. |
| ONPE | Resultados por mesa, segunda vuelta presidencial | 2021 | [Resultados por mesa — Segunda vuelta](https://www.datosabiertos.gob.pe/dataset/resultados-por-mesa-de-las-elecciones-presidenciales-2021-segunda-vuelta-oficina-nacional-de) | Publicación oficial localizada; versión exacta del archivo local pendiente de contrastar. |
| INEI | Mapa de Pobreza Provincial y Distrital | 2018 | [Mapa de Pobreza — compendio y anexos](https://www.gob.pe/institucion/inei/colecciones/6608-mapa-de-pobreza) | Año y publicación correspondientes; anexo exacto pendiente de contrastar. |
| PNUD | Índice de Desarrollo Humano e ingreso familiar per cápita | 2019 | [El reto de la igualdad](https://www.undp.org/es/peru/publicaciones/el-reto-de-la-igualdad) | Publicación de referencia correspondiente; tabla/archivo exacto pendiente de contrastar. |
| INEI | Códigos territoriales UBIGEO | Catálogo territorial | [Código de ubicación geográfica en el Perú](https://www.datosabiertos.gob.pe/dataset/c%C3%B3digo-de-ubicaci%C3%B3n-geogr%C3%A1fica-en-el-per%C3%BA-instituto-nacional-de-estad%C3%ADstica-e-inform%C3%A1tica) | Fuente oficial identificada; edición exacta del catálogo local pendiente de contrastar. |

## Archivos locales de trabajo

Los insumos originales se conservan localmente en `data/raw/`. Entre los nombres documentados para este proyecto figuran `Resultados_1ra_vuelta_Version_PCM.csv`, `Resultados_2da_vuelta_Version_PCM.csv`, `IDH-2019.xlsx`, `Anexo_Estadistico.xlsx` y archivos de UBIGEO. Estos nombres son referencias a los archivos de trabajo, **no enlaces de descarga**.

## Política de publicación y reproducibilidad

- Los datasets originales **no se redistribuyen** en este repositorio: `data/raw/`, `data/processed/` y `data/external/` están excluidos mediante `.gitignore`.
- El archivo `.pbix` permite examinar el modelo y las medidas en Power BI Desktop, pero para actualizar las consultas pueden requerirse los archivos fuente y la reconfiguración de rutas en Power Query.
- Las instituciones citadas son fuentes de información; no son autoras ni avalan el análisis o sus conclusiones.
- Las versiones exactas de algunos archivos originales **no se han verificado contra los recursos enlazados**. Esta limitación de trazabilidad debe considerarse al intentar reproducir el proyecto.
- Antes de redistribuir los datos o crear productos derivados, deben consultarse las condiciones de licencia y reutilización de cada publicación.

## Alcance metodológico

Los datos electorales son de 2021, mientras que la pobreza corresponde a 2018 y los indicadores de desarrollo humano a 2019. El indicador de pobreza utilizado es una aproximación basada en el punto medio del intervalo distrital. Las asociaciones estadísticas observadas a nivel de distrito **no implican causalidad ni permiten inferir conductas individuales**.

Consulta adicional: [Plataforma Nacional de Datos Abiertos del Perú](https://www.datosabiertos.gob.pe/).

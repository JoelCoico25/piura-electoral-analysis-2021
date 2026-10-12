# Fuentes de datos

El proyecto integra fuentes públicas de distintas instituciones. **Los archivos originales no se incluyen en el repositorio**; deben obtenerse de las entidades correspondientes y verificarse sus condiciones de reutilización.

| Institución | Información utilizada | Año de referencia |
|---|---|---|
| ONPE | Resultados electorales agregados por territorio, primera y segunda vuelta | 2021 |
| INEI | Indicadores / intervalos de pobreza distrital | 2018 |
| PNUD | Índice de Desarrollo Humano e ingreso familiar per cápita distrital | 2019 |
| INEI | Códigos UBIGEO y correspondencias territoriales | Catálogo empleado en el proyecto |

## Archivos locales de trabajo

En `data/raw/` se mantienen localmente archivos originales como `Resultados_1ra_vuelta_Version_PCM.csv`, `Resultados_2da_vuelta_Version_PCM.csv`, `IDH-2019.xlsx`, `Anexo_Estadistico.xlsx` y archivos de UBIGEO. Los nombres reflejan los insumos del proyecto, pero **no constituyen enlaces oficiales de descarga**.

## Política de publicación

- No se publican `data/raw/`, `data/processed/` ni `data/external/`.
- No se atribuye a las instituciones la autoría del análisis, las conclusiones o las visualizaciones.
- Para reproducir el dashboard, obtener los datasets desde sus portales oficiales y ajustar las rutas de origen en Power Query.
- Verificar las condiciones de uso y las versiones de cada fuente antes de reutilizar o redistribuir datos.

Portales institucionales de referencia: [ONPE](https://www.onpe.gob.pe/), [INEI](https://www.inei.gob.pe/) y [PNUD Perú](https://www.undp.org/es/peru).

> Pendiente para una versión de reproducibilidad completa: añadir las URL específicas de descarga y fecha de consulta de cada dataset, verificadas contra los archivos efectivamente utilizados.

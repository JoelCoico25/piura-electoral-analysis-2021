# Metodología y limitaciones

## Objetivo

Analizar las diferencias territoriales de participación y ausentismo en las dos vueltas de las elecciones presidenciales de Perú de 2021 en Piura y explorar sus asociaciones estadísticas con pobreza, desarrollo humano e ingreso familiar.

## Unidad de análisis y cobertura

- Unidad geográfica: **distrito**, identificado mediante UBIGEO.
- Cobertura: **65 distritos** de **8 provincias** del departamento de Piura.
- Dimensión temporal electoral: **primera y segunda vuelta de 2021**.
- Tabla electoral: **130 registros distrito-vuelta** (65 distritos × 2 vueltas).

## Integración y modelo

Se integraron resultados electorales de ONPE, información de pobreza distrital de INEI (2018), indicadores distritales de PNUD (2019) y códigos territoriales UBIGEO. El modelo de Power BI utiliza `DIM_TERRITORIO`, `FACT_PARTICIPACION`, `FACT_POBREZA_2018`, `FACT_DESARROLLO_2019` y una tabla de medidas DAX.

## Indicadores

- **Participación (%)** = 100 × total de votantes / total de electores hábiles.
- **Ausentismo (%)** = 100 × (total de electores hábiles − total de votantes) / total de electores hábiles.
- **Variación entre vueltas (pp)** = participación de segunda vuelta (%) − participación de primera vuelta (%).
- **Correlación de Pearson (r)**: asociación lineal entre indicadores socioeconómicos y ausentismo, calculada sobre distritos con datos válidos, sin duplicar distritos por la existencia de dos vueltas.

Las tasas agregadas se calculan a partir de **sumas de numeradores y denominadores**, no como promedios simples de porcentajes distritales.

## Hallazgos descriptivos

- Primera vuelta: **66,75 %** de participación.
- Segunda vuelta: **75,34 %** de participación.
- Variación: **+8,59 puntos porcentuales**.
- Correlaciones distritales en primera vuelta: pobreza estimada vs. ausentismo **+0,757**; IDH vs. ausentismo **−0,736**; ingreso familiar per cápita vs. ausentismo **−0,709**.

## Limitaciones

1. **Correlación no implica causalidad.** Los resultados no permiten atribuir el ausentismo a un factor concreto.
2. **Inferencia ecológica.** Los patrones entre distritos no permiten inferir cómo votó o por qué se ausentó una persona.
3. **Desfase temporal.** La información de pobreza (2018) y desarrollo (2019) precede a la elección (2021).
4. **Pobreza aproximada.** Se usa el punto medio de un intervalo de pobreza distrital, no una medición puntual observada.
5. **Variables omitidas.** Factores como accesibilidad a locales de votación, movilidad, contexto sanitario y otras características territoriales podrían estar asociados con la participación y no quedan aislados por este análisis descriptivo.
6. **Ámbito territorial.** Los resultados corresponden a Piura y no deben generalizarse automáticamente a otros departamentos.

## Independencia

Proyecto independiente y no partidista basado en datos públicos agregados. No representa a ONPE, INEI, PNUD ni a organizaciones políticas.

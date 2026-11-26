# Datos INE vía MCP oficial (`es-ine/mcp`)

Extraídos el **2026-11-26** con el servidor MCP institucional del INE ([github.com/es-ine/mcp](https://github.com/es-ine/mcp)), clonado en `tools/ine-mcp` y registrado en `~/.cursor/mcp.json`. Cada cifra sale de la API Tempus3; se cita operación, tabla y URL.

Raw: `data/ine_mcp_raw/`, `data/ine_vte_viviendas.json`, `data/ine_key_series.json`, `data/ine_summary.json`.

---

## Conseguido (mapeado a la lista de necesidades)

### B. Vacancy / stock (Censo 2011 — CENSOPV)

**Operación:** `CENSOPV` (id 8) · **Tablas:** [3457](https://www.ine.es/jaxiT3/Tabla.htm?t=3457) (CCAA/provincias), [3456](https://www.ine.es/jaxiT3/Tabla.htm?t=3456) (municipios >2k) · **Periodo:** 2011

| Ámbito | Total viviendas | Principal | Secundaria | Vacía | Tasa vacía |
| --- | ---: | ---: | ---: | ---: | ---: |
| España | 25 218 536 | 18 083 692 | 3 681 565 | 3 443 365 | **13,65%** |
| Madrid (CCAA) | 2 895 660 | 2 469 378 | 162 022 | 263 279 | **9,09%** |
| Barcelona (prov.) | 2 604 368 | 2 160 607 | 151 335 | 283 155 | **10,87%** |
| Barcelona (mun.) | 811 521 | 684 078 | 38 769 | 88 259 | **10,88%** |
| Alicante (prov.) | 1 274 325 | 738 367 | 326 705 | 209 024 | **16,40%** |
| Málaga (prov.) | 897 647 | 606 351 | 170 438 | 120 611 | **13,44%** |

Cubre ítems de lista: **#14** (tasa vacía), **#16** (principal/2ª/vacía), **#2** (stock), **#33** (2ªs), parte de **#38**.

> **Límite:** en la API Tempus3 de CENSOPV **no aparece** (en esta sesión) una tabla de vacías del **Censo 2021**. El ancla IEB ~12,3% ciudades >50k sigue siendo Censo 2011.

---

### D/E. Viviendas turísticas (VTE)

**Operación:** `VTE` (id 410) · **Tablas:** [39364](https://www.ine.es/jaxiT3/Tabla.htm?t=39364) (nº), [39365](https://www.ine.es/jaxiT3/Tabla.htm?t=39365) (% sobre censadas)

**Nº de viviendas turísticas** (serie experimental; varios puntos por año = distintos meses/cortes):

| Ámbito | Último punto 2026 | Pico reciente (aprox.) |
| --- | ---: | ---: |
| España | **341 001** | ~403 267 (2024) |
| Cataluña | 51 305 | ~58 705 (2024) |
| C. Valenciana | 51 268 | ~71 146 (2024) |
| Canarias | 48 356 | ~51 286 (2024) |
| Málaga (prov.) | 45 176 | ~48 412 (2025) |
| Alicante (prov.) | 32 148 | ~44 589 (2024) |
| Balears | 21 304 | ~26 979 (2024) |
| Barcelona (prov.) | 15 905 | ~18 690 (2024) |
| Madrid (CCAA) | 13 431 | ~22 435 (2024) |

**% sobre viviendas censadas** (último 2026): España **1,28%**; Cataluña 1,31%; Barcelona prov. 0,61%; Madrid 0,45%.

Cubre: **#36**, parte de **#39/#46**, refuerzo BdE “+50k turísticas”.

---

### A. Precios compraventa y alquiler

**IPV** — op. 15 · tabla [80270](https://www.ine.es/jaxiT3/Tabla.htm?t=80270) (trimestral)

| Ámbito | Índice (último) | Variación anual (última) |
| --- | ---: | ---: |
| Nacional | 111,1 | **+12,2%** |
| Madrid | 111,9 | **+12,9%** |
| Cataluña | 109,0 | **+10,1%** |

(Serie 2025–26 con varios trimestres; anuales ~+12–14% en Madrid.)

**IPVA** (alquiler) — op. 432 · tabla [59056](https://www.ine.es/jaxiT3/Tabla.htm?t=59056)

| Año | Índice nacional (Total) |
| --- | ---: |
| 2015 | 100,0 |
| 2020 | 110,9 |
| 2023 | 118,7 |
| **2024** | **122,9** |

→ alquileres ~**+23%** acumulado 2015–24 (índice).

**IRAV** — op. 481 · tabla [72975](https://www.ine.es/jaxiT3/Tabla.htm?t=72975): variación anual del índice de referencia de arrendamientos ~**2,1–2,6%** en puntos recientes 2025–26.

Cubre: **#4**, **#5**, parte de **#6**.

---

### A. Hogares / demografía

**ECP** — op. 450 · tabla [60131](https://www.ine.es/jaxiT3/Tabla.htm?t=60131)

- Hogares en viviendas familiares, Total Nacional (último): **19 953 529**
- Serie reciente: ~19,64M (2025) → ~19,95M (2026)

**PROH** — op. 70 · tabla [54562](https://www.ine.es/jaxiT3/Tabla.htm?t=54562): proyecciones de hogares disponibles (registrada; usar para gap vs stock).

Cubre: **#3** (parcial), complemento a gap oferta-demanda (el gap 400–450k es **BdE**, no INE).

---

### I. Tenencia / equity (ECV)

**ECV** — op. 155 · tabla [9997](https://www.ine.es/jaxiT3/Tabla.htm?t=9997) — % hogares por régimen de tenencia (Total Nacional):

| Régimen | 2025 | 2024 | 2023 |
| --- | ---: | ---: | ---: |
| Propiedad (total) | **73,3%** | 73,6% | 75,1% |
| Propiedad sin hipoteca | 48,9% | 48,8% | 48,7% |
| Propiedad con hipoteca | 24,4% | — | — |

También hay cortes CCAA (Madrid, Cataluña) y categorías de alquiler a/bajo mercado en la misma tabla.

Cubre: parte **#13**, **#75–76** (tenencia, no concentración de multi-propietarios).

---

### K. Transacciones / crédito (contexto mercado)

**ETDP** compraventas — tabla [6150](https://www.ine.es/jaxiT3/Tabla.htm?t=6150): vivienda nueva vs segunda mano vs libre (mensual 2026; p.ej. segunda mano ~39–48k/mes).

**Hipotecas** — tabla [76316](https://www.ine.es/jaxiT3/Tabla.htm?t=76316): hipotecas sobre **viviendas**, Total Nacional, ~**34–46k/mes** (2026).

Cubre: parte **#9** (flujo de mercado, no permisos/terminaciones MITMA).

---

## No está (o no salió) en el MCP/API INE

Estos ítems de la lista **no** se pueden cerrar solo con INE Tempus3 (hace falta BdE, MITMA, papers, Catastro, CCAA, etc.):

| Ítems lista | Por qué |
| --- | --- |
| #1 gap 400–450k hogares vs terminaciones | BdE Box 4 |
| #10 plazos permiso→obra | MITMA / sector |
| #11 elasticidad oferta | papers / estimaciones |
| #12 zonas tensionadas (mapa legal) | BOE / CCAA |
| #15 vacancy por duración (<6m…≥2a) | no en Censo API |
| #17–24 Francia TLV / Segú | papers / INSEE |
| #25–32 extrapolación FR→ES, enforcement, tax catalán | legal/policy |
| #34 días ocupación 2ªs | no INE estándar |
| #35 no residentes / compraventas extranjeros | BdE / Registradores |
| #37 contabilidad BdE 310k/390k | BdE |
| #41–45 Airbnb causal BCN | Garcia-López et al. |
| #47–54 parámetros modelo \(b_j\), real option | no estadística oficial |
| #55–68 calibración de *nuestra* medida | diseño propio |
| #69–73 externalidades blight | papers |
| #74, #77–78 concentración wealth / grandes tenedores | BdE / Catastro / CNMV |
| #80–82 capitalización ayudas, financiarización | papers / UCL |
| #83–88 elasticidades incidencia / evasión | estimaciones |
| #89–95 Auckland, Asquith, rent control | papers |
| #96–101 diseño legal vacancy tax | BOE / CCAA |
| #102–106 límites overclaim | papers |

**Censo 2021 vacías:** operación `CENSOP` (463) aparece en catálogo; **no** encontramos tabla de tipo de vivienda/vacías 2021 usable en el flujo MCP de esta sesión.

---

## Operaciones INE útiles para seguir tirando

| Código | Id | Para qué |
| --- | --- | --- |
| CENSOPV | 8 | Stock / vacías / 2ªs (hoy 2011) |
| VTE | 410 | Turísticas |
| IPV | 15 | Precios compraventa |
| IPVA | 432 | Precios alquiler |
| IRAV | 481 | Índice referencia alquiler |
| ECP / PROH | 450 / 70 | Hogares |
| ECV | 155 | Tenencia, pobreza×vivienda |
| ETDP / HPT | 7 / 40 | Compraventas / hipotecas |
| EH | 259 | Ejecuciones hipotecarias |
| EOAP / IPAP | 239 / 61 | Apartamentos turísticos ocupación/precios |
| IPCO / EEECN | 486 / 473 | Construcción |
| EM / EMCR / DPOP | 71 / 455 / 22 | Migración / padrón |
| UA | 10 | Indicadores urbanos |
| ADRH | 353 | Renta hogares (atlas) |
| APSH | 216 | Sin hogar (**coming soon** en catálogo MCP) |

---

## Setup (ya hecho en esta máquina)

```json
"ine": {
  "command": "uv",
  "args": ["run", "--directory", "/home/pedrojon/PublicEconomicsHousing/tools/ine-mcp", "ine-mcp"]
}
```

Reinicia Cursor / recarga MCPs si quieres las 5 tools (`ine_select_*`) dentro del Agent de forma nativa. Mientras, el harvest se hizo hablando al mismo servidor por stdio.

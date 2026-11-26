# Research Brief: Datos oficiales institucionales que faltaban

**Depth:** deep (acotado a *solo fuentes oficiales institucionales*)  
**Date:** 2026-11-26  
**Scope:** Rellenar los huecos de la lista de datos del proyecto vacancy tax / anti-grandes poseedores, **sin papers académicos** salvo cuando una institución publica el dato.  
**Complementa:** `docs/ine-data-from-mcp.md` (harvest Tempus3) + lista exhaustiva del chat.

## Executive Summary

Casi todos los huecos “duros” de diagnóstico ES (gap oferta-demanda, stock movilizable Madrid/BCN, Censo 2021 vacías, no residentes, construcción, grandes tenedores, diseño legal, vacantes FR, recaudación catalana) tienen **ancla institucional**. Lo que **no** existe como estadística oficial es: elasticidades, daño marginal Pigou, efecto causal del tax, y vacancy natural ~5% (literatura). Para el debate, el bloque BdE Box 4 + Censo 2021 + Catastro + BOE/ATC es suficiente para no depender de papers en el diagnóstico.

---

## 1. Mapa hueco → fuente → cifra

### 1.1 Diagnóstico demanda / gap (#1, #3, #37)

| Dato | Cifra oficial | Fuente |
| --- | --- | --- |
| Gap acumulado hogares vs terminaciones 2022–24 | **400 000–450 000** viviendas | BdE, *Informe Anual 2024*, Recuadro 4 |
| Creación neta hogares | ~**180 000** en 2024; promedio ~**245 000**/año en 2022–23 | BdE Box 4 (cita INE ECP) |
| Capacidad si se movilizan 2ªs + usos alternativos + vacías | **~390 000** hogares (Madrid) · **~310 000** (Barcelona) | BdE Box 4 |
| Stock no residencial / holgura vs hogares | Equivale a **~39%** de los hogares (nacional, heterogéneo) | BdE Box 4 |
| Vacías en municipios >250 000 hab. | Solo **~400 000** de ~4M vacías (dato 2020/Censo) | BdE Box 4, nota 15 (cita INE 2023) |

**URLs:**  
- https://www.bde.es/f/webbe/SES/Secciones/Publicaciones/PublicacionesAnuales/InformesAnuales/24/Fich/InfAnual_2024_Recuadros.pdf  
- Local: `references/policy/BdE_Annual_Report_2024_Boxes_EN.pdf`

---

### 1.2 Censo 2021 vacías / intensidad de uso (#14–16, #32, update vs 2011)

**Antes:** solo Censo 2011 vía Tempus3 (13,65% vacía).  
**Ahora (oficial INE, tabla 59531, actualizada 22/11/2024):**

| Ámbito | Totales | Vacías | % vacía | Uso esporádico | Bajo consumo |
| --- | ---: | ---: | ---: | ---: | ---: |
| **España** | 26 623 708 | **3 828 307** | **14,4%** | 2 517 628 (9,5%) | 941 637 (3,5%) |
| Madrid CCAA | 2 956 941 | 187 586 | **6,3%** | 186 655 | 53 978 |
| Madrid capital | 1 533 221 | 96 921 | **6,3%** | 100 087 | 27 228 |
| Barcelona prov. | 2 597 046 | 213 002 | **8,2%** | 166 090 | 50 219 |
| Barcelona ciudad | 808 751 | 75 488 | **9,3%** | 55 772 | 16 123 |
| Alicante prov. | 1 350 006 | 209 487 | **15,5%** | 163 228 | — |
| Málaga prov. | 996 557 | 152 843 | **15,3%** | 89 735 | — |
| Málaga ciudad | 261 857 | 16 541 | **6,3%** | 16 853 | — |

**Definición oficial (cambio metodológico crítico):** vacía = sin contrato eléctrico o consumo &lt; umbral municipal ≈ **15 días/año** de vivienda media local. “Uso esporádico” ≈ 251–750 kWh (~1–3 meses). **No** es la taxonomía principal/secundaria/vacía del Censo 2011 → **no comparar tasas a ciegas**.

NP INE: municipios pequeños concentran mucha vacía; ciudades &gt;250k tienen **poca** fracción del total de vacías (coherente con nota BdE de solo ~400k vacías en mun. grandes).

**URLs / archivo:**  
- Tabla: https://www.ine.es/jaxi/Tabla.htm?tpx=59531  
- CSV local: `data/ine_censo2021_intensidad_uso_59531.csv`  
- NP: https://ine.es/prensa/censo_2021_jun.pdf  

---

### 1.3 No residentes / extranjeros (#35)

| Dato | Cifra | Fuente |
| --- | --- | --- |
| Compraventas no residentes | **~8,4%** del total en 2024; ~**60 000**/año desde 2022 | BdE Box 4 |
| Stock viviendas de extranjeros no residentes | **&gt;500 000** (~**2%** del stock); ~**11%** Alicante, ~**8,5%** Málaga | BdE Box 4 |
| % compras extranjeros (residentes+no) | **14,6%** en 2024 (~93 000); Alicante **43,8%**, Baleares **32,6%**, Málaga **32,4%** | Colegio de Registradores, *ERI Anuario 2024* |
| Extranjeros no residentes (serie MIVAU/Notariado) | p.ej. **13 690** (3T24), **14 801** (4T24); pico **17 814** (2T22) | Serie institucional MIVAU (vía Notariado) |

**Cuidado:** Registradores = extranjeros totales (no separa residencia). BdE/MIVAU sí hablan de **no residentes**. Usar BdE para el claim “no residente”; Registradores para peso extranjero total.

---

### 1.4 Construcción / timing (#9–10, frente construction-led)

| Dato | Cifra | Fuente |
| --- | --- | --- |
| Viviendas iniciadas 2024 (VL+VP) | **136 187** (VL 112 220 + VP calif. prov. 23 967) | MIVAU, Observatorio Vivienda y Suelo, Boletín Anual 2024 |
| Viviendas terminadas 2024 | **100 980** (VL 86 609 + VP calif. def. 14 371) | Idem |
| Iniciadas / terminadas 2023 | 110 344 / 89 320 | Idem |
| Visados obra nueva 2024 (nota MIVAU) | **126 761** | Nota prensa MIVAU 20/03/2025 |
| Iniciadas 2025 (nota MIVAU jun-2026) | **137 330** | Nota MIVAU 23/06/2026 |

**URL portal:** https://www.mivau.gob.es/urbanismo-y-suelo/suelo/observatorio-de-vivienda-y-suelo  

**Uso debate:** terminaciones ~90–100k/año vs hogares ~180–245k → gap; vacancy tax actúa sobre stock **ya existente** (timing).

---

### 1.5 Grandes tenedores / concentración (#26–28, #74–78)

#### Catastro (DG Catastro, Hacienda) — titularidad residencial 2025  
Ámbito: **sin Navarra ni País Vasco**. Cuenta por sujeto pasivo IBI.

| Tramo viviendas/titular | Titulares | Viviendas |
| --- | ---: | ---: |
| 1 | 12 941 416 | 12 941 416 |
| 2–5 | 3 974 244 | 9 515 931 |
| 6–10 | 104 314 | 737 462 |
| **11–25** (gran tenedor Ley 12/2023) | 21 515 | 316 766 |
| **26–100** | 4 539 | 195 321 |
| **&gt;100** | 843 | 528 868 |
| **≥11 (suma “grandes”)** | **26 897** | **1 040 955 (~4,3% stock catastral)** |

Personas físicas ≈ **93%** de inmuebles residenciales; empresas ≈ **4,4%**.

**Portal:** https://www.catastro.hacienda.gob.es/es-ES/estadisticas_3_1.html  

#### BdE EFF 2022 (riqueza, no nº de pisos)

| Dato | Cifra | Fuente |
| --- | --- | --- |
| Propiedad vivienda principal | **72,1%** hogares (bajó desde 73,9% en 2020) | EFF 2022 |
| Otras propiedades inmobiliarias | **46,8%** hogares; **33,8%** tienen otra vivienda | EFF 2022 |
| Peso vivienda principal / otras props. en activos reales | **52,9%** / **35,7%** | EFF 2022 |
| Jóvenes &lt;35 propietarios | **31,8%** (era 69,3% en 2011) | EFF 2022 |
| Top 10% riqueza neta en riqueza vivienda | ~**36,7–38,5%** (series distributivas BdE) | BdE Boletín Económico 4/2023 |

---

### 1.6 Extrapolabilidad ES ↔ FR (#17–25)

| Dato | ES | FR | Fuente |
| --- | --- | --- | --- |
| Vacancy / logements vacants | **14,4%** vacías Censo 2021 (def. eléctrica) | **7,6%** métropole 2025 (2,849M); **7,7%** hors Mayotte | INE 59531 · INSEE Focus 359 |
| Unoccupied (vacant+2ªs) Census 2021 Eurostat | **30,4%** (8,09M / 26,6M) | **17,9%** (6,63M / 37,0M) | Eurostat Census 2021 (ocupancy) |
| Instrumento fiscal | Recargo IBI + impuesto CCAA (CAT) | TLV (zonas tendues); tipos actuales **17% / 34%** valor locatif; umbral **≥1 año** (reforma LF; histórico Segú era ≥2 años/tipos distintos) | Service-Public / CGI art. 232 |
| Datos vacance longue durée parc privé | — | LOVAC (Cerema/DGFiP): vacants &gt;2 años por comuna | data.gouv.fr LOVAC |

**Claim seguro:** ES tiene **más** stock no-usual-residence que FR (Eurostat unoccupied; INSEE vacancy ~7–8% vs INE vacías 14%).  
**Claim cuidadoso:** definiciones **no son idénticas** (eléctrica ES vs recensement/fiscal FR); no mezclar 14,4% con 7,6% como si fueran el mismo objeto.

---

### 1.7 Diseño legal / enforcement (#96–101, #30–31)

| Elemento | Contenido oficial |
| --- | --- |
| **Gran tenedor (estatal)** | Ley 12/2023 art. 3.k: &gt;10 inmuebles residenciales **o** &gt;1 500 m² (excl. garajes/trasteros); en tensionadas CCAA puede bajar a **≥5** | [BOE-A-2023-12203](https://www.boe.es/buscar/act.php?id=BOE-A-2023-12203) |
| **Recargo IBI desocupadas** | DF 3ª Ley 12/2023: desocupación &gt;2 años, mínimo **4** viviendas/titular; recargo hasta **150%** cuota líquida | Idem |
| **Impuesto CAT vacías** | Ley 14/2015: vacío permanente **&gt;2 años** sin causa; sujetos = **personas jurídicas** + fondos titulización + PF **grandes tenedores (&gt;15 viviendas)**; recaudación finalista vivienda protegida | [BOE-A-2015-9206](https://www.boe.es/buscar/act.php?id=BOE-A-2015-9206) · [ATC](https://atc.gencat.cat/es/tributs/impost-habitatges-buits/) |
| **Recaudación CAT** | **2,44 M€** (2023) · **7,01 M€** (2024, +188%) | Idescat (Dept. Economia i Finances) |
| **Open data CAT** | Nº viviendas vacías declaradas por municipio/ejercicio 2018–2024 | https://analisi.transparenciacatalunya.cat/d/w8kv-kmwv |

---

### 1.8 Turísticas (refuerzo #36; ya parcialmente en MCP)

BdE: **+~50 000** viviendas turísticas promedio 2024 vs 2023 (cita estadística experimental INE).  
INE VTE (MCP): stock nacional reciente ~**341k–403k** según corte.

---

## 2. Qué sigue **sin** dato oficial institucional

| Necesidad (lista) | Por qué no hay cifra institucional limpia |
| --- | --- |
| Vacancy “natural” ~5% | Benchmark teórico (Wheaton etc.), no serie oficial |
| Efecto causal TLV −13% | Evaluación académica (Segú); no es “dato” INSEE |
| Elasticidad participación / oferta alquiler a \(t\) | Estimación econométrica |
| MD Pigou / capitalización blight | Papers (Linden–Rockoff, etc.) |
| Días medios ocupación 2ªs | No hay estadística nacional estándar |
| Efecto del tax sobre rentas ES | No hay evaluación oficial del impuesto CAT/IBI |
| Plazos medios permiso→entrega en meses | No consolidado en un solo indicador MIVAU (hay proxies de flujo) |
| Fondos/SOCIMI × vacíos (cruce) | Catastro da tipología fiscal, no “vacío”×fondo en tabla pública fácil |
| Airbnb hosts multi-listing causal | Paper JUE, no INE |

Para estos: o se citan papers del source pack **como evidencia**, o se deja como supuesto de diseño.

---

## 3. Fuentes institucionales a usar (stack)

| Institución | Rol en el argumentario |
| --- | --- |
| **BdE** | Narrativa gap + movilización stock + no residentes + asequibilidad |
| **INE** | Censo 2021 intensidad uso; VTE; IPV/IPVA; hogares; ECV |
| **MIVAU** | Iniciadas/terminadas/visados; transacciones |
| **DG Catastro** | Distribución de titularidad / grandes tenedores |
| **BOE / ATC / Idescat** | Diseño legal + recaudación CAT |
| **Registradores / Notariado** | Compraventas extranjeros (complemento) |
| **Eurostat / INSEE** | Extrapolabilidad ES–FR (con matices de definición) |
| **Service-Public / data.gouv (TLV, LOVAC)** | Diseño y vacance longue durée Francia |

**Fuera de alcance de este brief (por petición):** press no institucional, think tanks privados, papers.

---

## 4. Claims listos (solo institucionales)

1. “El BdE cifra el déficit acumulado 2022–24 entre terminaciones y hogares en **400–450 mil** viviendas.”  
2. “Si se movilizasen 2ªs, usos turísticos/seasonal y vacías, Madrid podría absorber del orden de **390 mil** hogares y Barcelona **310 mil** (BdE 2024).”  
3. “Según el Censo 2021 (consumo eléctrico), hay **3,83 millones** de viviendas vacías (**14,4%**); en Madrid capital la tasa baja a **~6,3%**, en Barcelona ciudad **~9,3%** — la vacía está más en municipios pequeños.”  
4. “Más de **500 mil** viviendas son de extranjeros no residentes; las compras de no residentes son ~**8,4%** del total (BdE).”  
5. “El Catastro cuenta **~27 mil** titulares con **más de 10** viviendas residenciales, con **~1,04 millones** de inmuebles (~4% del stock catastral común).”  
6. “Francia tiene ~**7,6%** logements vacants (INSEE 2025) frente a un unoccupied Eurostat 2021 de **17,9%** FR vs **30,4%** ES.”  
7. “Catalunya ya grava vacíos ≥2 años a personas jurídicas/grandes tenedores; recaudó **7 M€** en 2024 (Idescat).”  
8. “En 2024 se terminaron ~**101 mil** viviendas (MIVAU) frente a una creación de hogares mucho mayor — la vía stock es el complemento de timing.”

---

## 5. Riesgos / open questions

1. **Censo 2011 vs 2021:** no usar 13,7% y 14,4% como “subió la vacía” sin explicar el cambio de método.  
2. **Vacía en ciudades grandes es baja** → el claim anti-especulación debe apoyarse más en **2ªs + STR + no residentes + multi-propietarios**, no solo en “hay millones de vacías en Madrid centro”.  
3. **Recaudación CAT 7 M€** es pequeña → argumentar **comportamiento + finalismo**, no “financia el parque público sola”.  
4. **TLV Francia actual** (1 año, 17/34%) ≠ diseño Segú 1999 → para evidencia causal seguir citando el paper; para diseño, Service-Public.  
5. Cifras Catastro “grandes tenedores” usadas arriba vienen del fichero oficial de titularidad; conviene **descargar el Pc-Axis/CSV del portal** para la slide (evitar intermediarios).

---

## 6. Fases sugeridas (uso del pack de datos)

1. **Slides diagnóstico:** BdE gap + 310k/390k + Censo 2021 tabla ciudades.  
2. **Slides anti-grandes:** Catastro tramos + definición Ley 12/2023 + ATC CAT.  
3. **Slides extrapolación:** INSEE vacancy + Eurostat unoccupied ES/FR + diseño TLV.  
4. **Vs construction:** MIVAU terminaciones vs hogares BdE/INE.  
5. **Pendiente opcional:** CSV open data ATC viviendas declaradas; LOVAC FR &gt;2 años; serie MIVAU no residentes completa.

---

## 7. Reusable from this repo

| Artefacto | Uso |
| --- | --- |
| `docs/ine-data-from-mcp.md` | IPV, IPVA, VTE, ECV, hogares (Tempus3) |
| `data/ine_censo2021_intensidad_uso_59531.csv` | Vacías 2021 por mun/prov |
| `references/policy/BdE_*` | Box 4 PDF ya local |
| `tools/ine-mcp` | Re-consultar series INE |

---

## Sources (institucionales)

- Banco de España, Informe Anual 2024, Recuadro 4  
- INE, Censos 2021 — viviendas según intensidad de uso (tpx 59531) + NP 30/06/2023  
- MIVAU, Observatorio de Vivienda y Suelo, Boletín Anual 2024 (+ notas 2025/2026)  
- Dirección General del Catastro, Estadísticas de titularidad  
- BdE, Encuesta Financiera de las Familias 2022 (DO 2413) + Boletín Económico 4/2023  
- BOE: Ley 12/2023; Ley 14/2015 (CAT)  
- ATC / Idescat: impuesto viviendas vacías, recaudación  
- Colegio de Registradores, ERI Anuario 2024  
- INSEE Focus 359 (parc logements 2025)  
- Eurostat Census 2021 occupancy metadata + series unoccupied  
- Service-Public F17293 (TLV); data.gouv LOVAC / zonage TLV  

---

## Competitive Landscape / Ecosystem / Libraries

*N/A — este brief no es product discovery; es inventory de datos oficiales para un debate de Public Economics.*

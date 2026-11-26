# Argumentos, modelos y lógicas a favor del impuesto a viviendas vacías

Documento de trabajo para la posición **anti-grandes poseedores / vacancy tax**. Extrae de las fuentes en `references/` lo que **apoya directamente** la medida, lo que se puede **extrapolar** con cuidado, y cómo **gestionar** los papers del lado construction/supply en el debate.

**Nuestra medida (núcleo):** impuesto sobre vacancy prolongada, con umbrales/énfasis en multi-propietarios y grandes poseedores; uso de recaudación hacia vivienda asequible / limited-profit; complementary a (no sustituto de) oferta nueva.

---

## 1. Mapa rápido: qué paper para qué claim

| Claim que queremos hacer | Fuente ancla | Tipo de apoyo |
| --- | --- | --- |
| Vacancy voluntaria es un fenómeno económico racional, no “error estadístico” | Segú (2020); IEB 2/2018 | Modelo + teoría |
| Vacancy por encima de la “natural” justifica intervención | IEB 2/2018 (España ~12% vs ~5%) | Benchmark empírico |
| Un vacancy tax **reduce** vacancy (sobre todo long-term) | Segú (2020): −13% | Causal DiD+PSM |
| Las unidades vuelven a **uso residencial primario** | Segú (2020) | Mecanismo empírico |
| Es **más rápido** movilizar stock que construir | Segú (2020); slides BdE | Argumento de timing |
| Externalidades negativas de vacíos → caso de eficiencia, no solo equity | Segú intro (Lee, Immergluck, Glaeser…) | Teoría + evidencia secundaria |
| Distorsiones previas (tenant protection, real options) justifican place-based tax | Segú citando Kline & Moretti (2014) | Lógica de second-best |
| Airbnb/STR desvía stock residencial → precios/rentas ↑ | Garcia-López et al. (2020) | Causal ES (BCN) |
| Demanda no residencial / turística / no residentes aprieta mercados ES | BdE Box 4 (2024) | Datos oficiales |
| Mobilizar 2ªs + turísticas + vacías liberaría capacidad en Madrid/BCN | BdE Box 4 | Contabilidad de stock |
| Impuestos a demanda especulativa + vivienda pública > subsidios a compradores | Ryan-Collins / UCL (2024) | Argumento de política |
| Subsidios/allowances de demanda pueden **inflar** precios si oferta rígida | Segú lit. review (Fack, Laferrère…) | Contra-alternativa fiscal |
| Construcción nueva baja rentas *locales* (no niega vacancy tax) | Asquith et al. | Complementariedad / no exclusión |
| Upzoning aumenta permisos (no niega vacancy tax) | Greenaway-McGrevy & Phillips | Distinguir *consents* vs uso del stock |

---

## 2. Núcleo teórico: por qué hay vacíos y por qué un tax funciona

### 2.1 Dos tipos de vacancy (Segú 2020; IEB 2/2018; slides)

Lógica central del paper estrella:

1. **Frictional / open vacancies (v)**  
   - Surgen de *search & matching*: heterogeneidad de viviendas, costes de transacción, incertidumbre y negociación.  
   - Son involuntarias: el propietario *quiere* alquilar/vender pero tarda en emparejar.  
   - En equilibrio hay un nivel positivo de vacancy estructural (análogo a la tasa natural de paro) — Wheaton (1990). Estimaciones típicas ~5%.

2. **Inactive / voluntary vacancy (i)**  
   El propietario **elige** no participar en el mercado. Dos mecanismos:
   - **Real option / uncertainty** (Cunningham 2006): con incertidumbre de precios, esperar tiene valor; retrasar venta/alquiler puede ser óptimo privado.  
   - **Strategic holding** bajo regulación pro-inquilino (Gabriel & Nothaft 2001): si no puedes ajustar renta ni terminar contratos fácilmente, puede ser racional sacar la unidad del alquiler.

**Total medido:** \(V = v + i\).

**Extrapolación a nuestra posición:** grandes poseedores / inversores son los agentes para los que \(b_j\) (outside option de dejar vacío) es sistemáticamente alto: option value de plusvalía, cartera diversificada, menor urgencia de cash-flow. Un tax apunta a ese margen.

### 2.2 Modelo de participación (Segú sobre Desgranges & Wasmer 2000)

Setup (parcial equilibrio, corto plazo, stock fijo):

- Propietarios eligen participar o no según: valor de tener la unidad en el mercado vs outside option \(b_j\) **menos el impuesto \(t\)**.
- Condición de participación: \(rV_j \ge b_j - t\).
- Subir \(t\) eleva el umbral \(b^*\): menos unidades inactivas.
- Predicciones del modelo:
  - \(i \downarrow\) (inactive stock cae)
  - \(v \uparrow\) algo (más open vacancies al entrar al matching)
  - \(V = v+i \downarrow\) neto (la caída de \(i\) domina)
  - Rentas: presión a la baja en el **corto plazo** (más bargaining power de demandantes / mayor coste de oportunidad de no alquilar)
  - Largo plazo: posible efecto adverso sobre inversión/nueva construcción (limitación del modelo ST)

**Lógica usable en 10′:** el impuesto no “castiga fricciones”; castiga **no participar**. Quien oferta de verdad puede estar exento (diseño francés: si demuestras que intentas alquilar/vender). Eso alinea con enforcement serio y con no golpear al pequeño propietario en transición.

### 2.3 Justificación de intervención pública (eficiencia + equity)

Segú articula **dos** justificaciones (ambas sirven):

| Canal | Lógica | Cómo lo usamos |
| --- | --- | --- |
| **Equity / asequibilidad** | Con demanda alta y oferta inelástica, vacancy high es paradoxal; movilizar stock redistribuye capacidad residencial | “No hace falta esperar a que se construya: hay viviendas que ya existen” |
| **Eficiencia / externalidades** | Concentraciones de vacíos → ↓ valor de vecinos, inseguridad, delincuencia, cohesión (Lee; Immergluck & Smith; Ellen; Glaeser et al.) | Caso Pigouviano: el vacío impone coste social no internalizado |
| **Second-best / place-based** | Si hay distorsiones previas (tenant protection, real options), un tax place-based puede compensarlas (Kline & Moretti 2014) | En ES: Ley de vivienda / protección de inquilinos + plusvalías → inactive stock plausible |

**Timing argument (muy fuerte frente a construction-led):**  
> “Focusing on vacancy reduction may be a faster and easier way to increase residential capacity than promoting the construction of new housing units.” (Segú 2020)

---

## 3. Evidencia causal del vacancy tax (Segú 2020)

### 3.1 Diseño institucional (Francia, TLV 1999) — plantilla de diseño

| Parámetro | TLV Francia | Implicación para nuestra propuesta |
| --- | --- | --- |
| Definición | Vacío de muebles ≥ **2 años** | Umbral temporal = ataca long-term / especulación, no rotación friccional |
| Tipo | 10% valor locativo (año 1) → 12.5% → 15% | Escala creciente = más cara cuanto más se alarga la vacancy |
| Ámbito | Unidades urbanas >200k con desequilibrio oferta-demanda | Focalizar mercados tensionados (Madrid, BCN, costas, islas) |
| Exención | Si se ofrece en alquiler/venta; obras mayores | Evita castigar matching honesto / reforma |
| Resultado clave | Vacancy ↓ **0.8 pp ≈ 13%** (1997–2001) | Ancla empírica #1 |
| Heterogeneidad | Efecto **~50% mayor** donde vacancy inicial era alta | Justifica targeting de hotspots |
| Margen | Concentrado en **long-term vacancy** | Encaja con “anti-especulación / grandes poseedores” |
| Destino de unidades | Mayoría → **primary residences** | No solo “cambio de etiqueta” a 2ª residencia (en Francia) |
| Construcción nueva | Sin efecto significativo a medio plazo | Contra el miedo “mata la oferta nueva” en el horizonte del debate |

### 3.2 Claims seguros vs claims cuidadosos

**Seguros (decir en la presentación):**
- Hay evidencia cuasi-experimental de que un vacancy tax reduce vacancy.
- El efecto es mayor en long-term vacancy y en municipios con más vacíos previos.
- Las unidades tienden a pasar a residencia principal.

**Cuidadosos (no exagerar):**
- Segú **no** estima un efecto grande y limpio de ↓ rentas a corto plazo en todos los specs; el modelo lo predice, la evidencia de precios es más mixta/largo plazo. Mejor claim: “libera stock residencial / reduce inactive housing”, no “bajará el alquiler un X% mañana”.
- Extrapolación Francia → España no es automática (medición, enforcement, 2ªs residencias). Ver §7.

### 3.3 Catalonia / España en IEB (diseño ya existente)

IEB 2/2018 (Segú) señala:

- España (Censo 2011): vacancy ~**12.3%** en ciudades >50k → por encima de la “natural” (~5%).
- Catalunya (desde 2015): tax a vacíos ≥2 años, **solo a personas jurídicas**, con reducción si se destina a asequible; recaudación a vivienda social.
- Problema histórico: IBI +50% a desocupados existe en teoría (TRLHL) pero municipios no podían definir “desocupado” → enforcement fallido (salvo País Vasco, etc.).

**Extrapolación anti-grandes poseedores:** el diseño catalán (legal entities) ya apunta a fondos/sociedades. Nuestra posición puede **generalizar y endurecer** ese principio: umbrales por nº de viviendas / personas jurídicas / carteras, no castigar la 1ª vivienda vacía por herencia reciente.

---

## 4. Airbnb / uso turístico: stock desviado del uso residencial

### 4.1 Garcia-López, Jofre-Monseny, Martínez-Mazza & Segú (2020)

**Lógica económica:**
- STR “ocasional” (piso vacío en vacaciones) puede ser eficiencia.
- STR **permanente** (pasar de alquiler de largo plazo a turístico) = ↓ oferta residencial → ↑ rentas y precios.

**Evidencia BCN (causal, varias estrategias):**
- Barrio medio: rentas **+1.9%**, precios transacción **+4.6%**, posted **+3.7%**.
- Top decil Airbnb: rentas **+7%**, precios **+17% / +14%**.
- En 2015, ~2% del stock en Airbnb; ~7% de las unidades en alquiler; con ~10 días/mes de Airbnb se igualaba la renta mensual de largo plazo (incentivo potente a desviar).

**Cómo lo usamos (sin abandonar vacancy tax):**
1. Muestra que el problema no es solo “faltan ladrillos”, sino **asignación del stock existente**.
2. Vacancy tax + reglas/fiscalidad STR son complementarios: ambos atacan el uso no residencial prolongado.
3. Grandes poseedores / hosts multi-listing son el margen intensivo (misma narrativa anti-concentración).

**BdE Box 4 refuerza el dato ES actual:** +~50 000 viviendas turísticas en 2024 vs 2023; presión en centros y zonas turísticas.

---

## 5. Datos españoles (BdE): desajuste y stock “infrautilizado”

### 5.1 Diagnóstico compatible con nuestra vía

De **Box 4, Informe Anual 2024**:

- Demanda robusta: demografía/migración, creación de hogares, no residentes (~8.4% de compraventas), macro favorable.
- Oferta nueva rezagada: gap acumulado 2022–24 de **400–450k** viviendas (completions vs hogares).
- Pero también: el stock total tiene **holgura contable** si se movilizan usos no residenciales.

Punto especialmente explotable:

> En Barcelona/Madrid, si se movilizasen 2ªs residencias + usos alternativos (turístico/seasonal) + (en menor medida) vacías, la capacidad podría absorber del orden de **310k hogares (BCN)** y **390k (Madrid)**.

Y:

> El aumento de alquileres de temporada / habitaciones / turísticos **limita** el crecimiento de la oferta de alquiler residencial.

**Lógica de debate:**
- El equipo construction-led usará el gap 400–450k → “hay que construir”.
- Nosotros: (a) construir es lento y cara; (b) parte del “shortage” es **uso del stock** (BdE lo cuantifica); (c) vacancy tax ataca precisamente ese margen, más barato y más rápido.

### 5.2 No residentes y 2ªs como “vacancy de facto”

IEB: en Madrid/BCN, ~10% vacías + ~4% 2ªs; las 2ªs son ocupación temporal muy corta → “sort of vacant units”.  
BdE: >500k viviendas de extranjeros no residentes; ratios altísimos en Alicante/Málaga/islas.

**Extrapolación de diseño:**  
Vacancy tax puro puede ser insuficiente donde el problema es 2ª residencia / turístico declarado. Propuesta coherente anti-grandes poseedores:

1. Vacancy tax (prolongada, enforcement fuerte).  
2. Recargo a 2ªs / no residentes / STR permanente (misma familia fiscal).  
3. Recaudación → vivienda pública / limited-profit.

Ryan-Collins (UCL): explícitamente recomienda **property taxes on speculative demand, including second homes**, + inversión pública directa — no subsidios hipotecarios a demandantes (que capitalizan en precio).

---

## 6. Argumentos de política / financiarización (Ryan-Collins)

### 6.1 Claims utilizables

| Claim | Uso |
| --- | --- |
| Vivienda + crédito crean ciclo de financiarización (homes as assets) | Framing: el vacío/especulación es síntoma de tratar la vivienda como activo |
| Subsidios a compradores (Help-to-Buy style) **inflan** precios | Atacar alternativas “pro-mercado” que suenan amables pero capitalizan |
| Mejor: **vivienda pública asequible** + **impuestos a demanda especulativa / 2ªs** | Encaja exactamente con vacancy tax + use of revenues |

### 6.2 Conexión con literature de allowances (Segú)

Segú resume evidencia de que ayudas a la demanda con oferta inelástica desplazan el beneficio al propietario (Fack 2005; Laferrère & Le Blanc; etc.).  
**Extrapolación:** en mercado tensionado ES, priorizar instrumentos que **aumenten oferta efectiva** (vacancy → uso; o construcción pública) frente a transferencias que se capitalizan.

---

## 7. Diseño: lecciones de enforcement y welfare (IEB + Segú)

### 7.1 Condiciones para que el tax mejore asequibilidad

IEB lista el balance de welfare:

| Factor | Efecto |
| --- | --- |
| Quién ocupa las ex-vacías | Si pasan a residencia primaria de hogares → gana asequibilidad; si solo se relabelan como 2ª → no |
| Uso de la recaudación | Reinvertir en vivienda social/asequible amplifica el efecto (ej. Catalunya) |
| Distorsión LT a inversión | Teoría: puede ↓ construction; empiria francesa: no se ve a medio plazo |
| Calidad / obras | Exenciones por reforma evitan castigar rehabilitación |
| Medición | Sin definición legal operable de “vacío”, el tax muere (problema ES clásico) |

**Implicación para slides:** dedicar 1 slide a **definición + enforcement + exenciones + uso de ingresos**. Eso es lo que el brief pide y lo que convierte un slogan en “government proposal”.

### 7.2 Extrapolación a “anti-grandes poseedores”

Lógicas que podemos defender sin traicionar los papers:

1. **Incidencia esperada:** el coste del tax es más alto para quien mantiene muchas unidades inactivas → cartera grande.  
2. **Heterogeneidad del efecto (Segú):** más impacto donde vacancy inicial es alta → mercados tensionados / stock retenido.  
3. **Personas jurídicas / umbrales** (Catalunya): diseño ya orientado a no pegar al propietario de una sola vivienda.  
4. **Complemento STR/2ªs:** grandes operadores están sobrerrepresentados en multi-listing y carteras de inversión.

Cuidado: Segú **no** identifica causalmente “fondos buitre” vs pequeños. No inventar ese resultado; argumentarlo como **diseño de incidencia**, no como hallazgo del paper.

---

## 8. Papers del otro lado: cómo no suicidarnos (y cómo girarlos)

### 8.1 Greenaway-McGrevy & Phillips (2023) — Auckland upzoning

- Hallazgo: upzoning ↑ construcción (permisos); robusto a displacement effects.  
- **No refuta** vacancy tax.  
- Respuesta parlamentaria:
  1. Distinguir **permitted** vs **completed** homes (el propio syllabus lo dice).  
  2. Timing: construcción tarda años; vacancy tax actúa sobre stock ya existente.  
  3. Complementariedad: “No estamos en contra de construir; priorizamos movilizar stock **y** no tratamos upzoning como solución única”.  
  4. Auckland ≠ España en elasticidad, turismo, 2ªs, financiarización.

### 8.2 Asquith, Mast & Reed — new apartments ↓ rentas cercanas

- Hallazgo: edificios nuevos market-rate ↓ rentas locales 5–7%; absorben hogares de renta alta.  
- Uso **a favor nuestro (parcial):** confirma que ↑ oferta efectiva baja rentas — exactamente la lógica de liberar vacíos al mercado.  
- Diferencia: ellos hablan de **nueva construcción**; nosotros de **oferta efectiva del stock**. Misma microeconomía de supply shock, distinto instrumento y horizonte.  
- No conceder: “entonces solo hay que construir”. Conceder: “la oferta importa; la más rápida es la que ya está vacía”.

### 8.3 Jofre–Martínez–Segú (2023) — rent control Catalunya

- Rentas −4% a −6%; sin evidencia clara de ↓ supply de contratos en su ventana.  
- **No es nuestro instrumento**, pero sirve para:
  - Mostrar que políticas “anti-mercado puro” pueden funcionar en ES bajo diseño fuerte.  
  - Advertir: rent control y vacancy tax interactúan (Segú: fuerte protección de inquilinos puede **aumentar** voluntary vacancy → el tax es el complemento second-best).  
- Si el parlamento propone solo rent control: “sin movilizar vacíos, caps pueden coexistir con stock inactivo; el tax ataca esa holgura”.

### 8.4 Chay–Greenstone / Linden–Rockoff (lectures)

- Capitalización: precios revelan WTP por amenities / riesgos.  
- Uso lateral: externalidades de vacancy (inseguridad, blight) se capitalizan en vecinos → argumento de eficiencia Pigouviana.  
- No forzar: no son papers de vacancy tax.

---

## 9. Cadena causal sugerida para la presentación (10′)

```
Demanda alta + oferta nueva lenta (BdE)
        +
Stock desviado: vacíos, 2ªs, STR (BdE + Airbnb BCN)
        +
Incentivos privados a retener vacío (real option / strategic holding)  [Segú modelo]
        ↓
Fallo: inactive housing + externalidades + equity
        ↓
Vacancy tax (t) eleva coste de no participar  [participación bj − t]
        ↓
i ↓ → V ↓ (esp. long-term) → primary residences ↑  [Segú empiria −13%]
        ↓
Oferta efectiva residencial ↑ (rápido) + recaudación → vivienda asequible
        ↓
Mejor acceso low/middle income; incidencia sobre grandes carteras inactivas
```

**Frente al otro gobierno (construction-led):**  
Misma crisis, distinto *binding constraint* en el corto plazo: no solo “permisos”, sino **incentivos de uso del stock**. Construcción es complemento; vacancy tax es el instrumento que defendemos como prioridad.

---

## 10. Frases / claims listos (con ancla)

1. “En Francia, el primer evaluation cuasi-experimental de un vacancy tax encuentra una caída del **13%** en la tasa de vacíos, concentrada en vacancy de largo plazo, con desplazamiento hacia residencias principales.” — Segú *JPubE* 2020.  
2. “Con oferta casi fija a corto plazo, gravar el vacío aumenta el coste de oportunidad de no alquilar y, en el modelo de search-and-matching, reduce el stock inactivo.” — Segú / Desgranges–Wasmer.  
3. “España lleva años con vacancy urbana por encima de la tasa ‘natural’ (~5% vs ~12% en ciudades grandes, Censo 2011).” — IEB 2/2018.  
4. “Airbnb en Barcelona no es anecdótico: en barrios del top decil, rentas +7% y precios hasta +17%.” — Garcia-López et al. *JUE* 2020.  
5. “El BdE cuantifica que movilizar 2ªs, usos turísticos/seasonal y vacíos liberaría cientos de miles de hogares potenciales en Madrid y Barcelona.” — Box 4, 2024.  
6. “Los subsidios a la demanda en mercados rígidos tienden a capitalizarse en precios; mejor gravar demanda especulativa y reinvertir en vivienda asequible.” — lit. allowances en Segú + Ryan-Collins/UCL.

---

## 11. Lo que *no* debemos decir (trampas)

- “Segú demuestra que bajan los alquileres un X% en España.” (No lo demuestra para ES; el paper es Francia y el foco principal es vacancy rate.)  
- “Upzoning no funciona.” (El paper de Auckland dice que sí aumenta construcción; atacar exclusividad, no existencia.)  
- “Asquith prueba que construir no ayuda.” (Prueba lo contrario a escala local.)  
- “Todos los vacíos son especulación de fondos.” (Parte es fricción; por eso el umbral de 2 años + exenciones.)  
- “El tax no tiene costes.” (Teoría LT: posible ↓ inversión; hay que admitir el trade-off y anclarlo en evidencia de medio plazo francesa + reinversión de ingresos.)

---

## 12. Fuentes usadas en este documento

- Segú (2020) *JPubE* + MPRA 2018 + slides BdE 2019 + IEB Report 2/2018  
- Garcia-López et al. (2020) *JUE* Airbnb Barcelona  
- BdE Annual Report 2024 Boxes (Box 4) + Annual Report 2023 (contexto)  
- UCL / Ryan-Collins (Sep 2024)  
- Greenaway-McGrevy & Phillips (2023); Asquith–Mast–Reed (WP); Jofre–Martínez–Segú (2023)  
- Chay–Greenstone; Linden–Rockoff (solo lógica de capitalización/externalidades)

Archivos locales: ver `references/REFERENCES.md`.

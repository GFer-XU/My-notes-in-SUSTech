# Environmental Monitoring · Final-Exam Review Notes (Systematic Edition)

> Scope: SUSTech *Environmental Monitoring* (Dr. Yuanyuan Tang), Chapters 2–7, covering the five domains — **water, air, solid waste, soil, and physical pollution**.
> How to use: Read **Part 0** first to build the framework → use **Part 1** to memorize the skeleton of each domain → use **Part 2** to weave the scattered instruments/methods into a network → focus on the procedures and calculations in **Part 3** → use **Parts 4–5** for last-minute gap-filling and high-frequency memorization.
>
> 📌 Chapter mapping: Ch.2 Water / Ch.3 Air & Waste Gas / Ch.4 Solid Waste / Ch.5 Soil / **Ch.7 Physical Pollution** (the lecture filename says "Chapter 6," but the content title is "Chapter 7 Physical Pollution Monitoring," which matches the textbook numbering — they are the same material).

---

# Part 0　Big Picture & Exam Map

## 0.1 "Environmental Monitoring" in one sentence

Environmental monitoring = **the whole process of measuring the types, concentrations, distribution, and trends of pollutants (and physical factors) in the environment in order to judge environmental quality.** It is not simply "doing experiments" — it is a **complete workflow chain**. In the exam, almost every long-answer question can be hung onto this chain.

## 0.2 The monitoring workflow chain (universal procedure — memorize it)

```
Define monitoring objective
   ↓
Determine monitoring target / parameters
   ↓
Site layout / station setup (sampling-point design)
   ↓
Sample collection → on-site measurement (flow / meteorology, etc.)
   ↓
Sample preservation / transport
   ↓
Sample pretreatment (digestion / enrichment / separation / extraction)
   ↓
Analytical determination (choose instrument & method)
   ↓
Data processing / result expression
   ↓
Quality Assurance & Quality Control (QA/QC, runs through the whole process)
   ↓
Evaluation (compare with standards, compute indices, classify)
```

> **Answer template:** For any short-answer question like "how to design a monitoring program for ××" or "how to monitor ××," expand along "objective → data collection → parameters → site layout → sampling time & frequency → sampling & analytical methods → result expression & QA/QC." You will rarely lose major points.

## 0.3 The "five elements + result" analytical framework

Any monitoring domain can be broken into the following 6 handles. Part 1 of these notes uses exactly this to build side-by-side "framework cards" for the five domains.

| Element | The question it answers |
|---|---|
| ① Monitoring objective | Why measure? (status / surveillance / emergency / management / research / arbitration) |
| ② Monitoring target | Which medium? (surface water / groundwater / wastewater; ambient air / waste gas; solid waste / hazardous waste; soil; sound / light / radiation) |
| ③ Monitoring parameters | Which indicators? (often classified as required/optional, Class I / Class II, basic items, etc.) |
| ④ Layout & sampling | Where, how, when, and how much to sample? |
| ⑤ Technique & instrument | Which method and instrument to use? |
| ⑥ Result & evaluation | How to compute, express, compare against which standard, and classify? |

## 0.4 Whole-course knowledge map (master table)

| Domain | Core targets | Signature indicators | Signature layout method | Signature instruments/methods | Key standard |
|---|---|---|---|---|---|
| **Water** | Surface water / groundwater / wastewater / sediment / activated sludge | DO, COD, BOD₅, ammonia-N, total P, heavy metals | River "reference–control–reduction" cross-sections | Spectrophotometry, AAS, ICP-OES, iodometry, dichromate method | GB3838-2002 Surface Water |
| **Air / waste gas** | Ambient air / indoor / stationary source / mobile source | SO₂, NOₓ, CO, O₃, PM₁₀/PM2.5, TSP | Grid / concentric-circle / sector layout | Spectrophotometry, GC, NDIR, gravimetry | GB3095 Ambient Air Quality |
| **Solid waste** | Industrial solid waste / hazardous waste / municipal refuse | Flammability/corrosivity/reactivity/toxicity (leaching toxicity, acute toxicity LD₅₀) | Diagonal / plum-blossom / checkerboard / S-shape | Leaching test, LD₅₀, calorific value (calorimeter) | GB5085 Hazardous Waste ID |
| **Soil** | Farmland / contaminated-site soil | Heavy metals, BHC/DDT, benzo(a)pyrene, background value | Diagonal / plum-blossom / checkerboard / S-shape / radial / grid | Mixed-acid digestion, AAS/ICP, GC, XRF | GB15618 Soil Quality |
| **Physical** | Noise / vibration / radioactivity / light | Sound pressure level Lp, equivalent level Leq, dose equivalent | (Noise) grid of measurement points | Sound level meter, dosimeter | GB3096 Acoustic Environment |

## 0.5 Quick scan of high-frequency exam points (to get oriented)

- **Concept distinctions:** primary/secondary pollutant, grab/composite water sample, acidity/alkalinity/pH, total N/Kjeldahl N, BOD/COD/TOC relationship, true color/apparent color, TSP/PM₁₀/PM2.5, α/β/γ decay, sound power/intensity/pressure.
- **Procedures:** river cross-section layout (reference/control/reduction), the three air-layout methods, soil-layout methods, solid-waste increment count and the quartering method, post-sampling preservation methods.
- **Calculations** (where you most easily lose — and gain — points): BOD (dilution method, seeding correction), DO (iodometry), COD (dichromate/coulometric), noise addition and subtraction, equivalent level, AQI/sub-indices, sound pressure level, half-life and dose, calorific-value conversion, standard-gas preparation, soil pollution index.
- **Method–pollutant pairing:** which pollutant uses which instrument/method (see the two master tables in Part 2).
- **Cases:** Minamata disease (Hg), Love Canal / Times Beach (hazardous waste / dioxin), Los Angeles photochemical smog.

---

# Part 1　Systematic Frameworks for the Five Monitoring Domains

> Each domain gets one "framework card," organized by the 6 elements in §0.3. Memorize the cards first, and your short-answer questions will have a skeleton.

## 1.1 Water Quality Monitoring (Chapter 2)

**① Monitoring objectives (6 types — commonly tested as "list them")**
1. Surface water — **routine monitoring**: grasp the current status and trends of water quality.
2. Production/daily processes — **surveillance (compliance) monitoring**: grasp wastewater discharge volume, pollutant concentration, and total discharge; evaluate compliance.
3. Accidents — **emergency monitoring**: analyze cause, harm, and countermeasures.
4. Environmental management — **provide data** for setting standards, regulations, and planning.
5. Environmental research — **provide baseline data** for quality assessment and forecasting.
6. Pollution disputes — **arbitration monitoring**: provide scientific evidence.

**② Monitoring targets:** environmental water bodies (rivers, lakes/reservoirs, groundwater, seas) + pollution sources (domestic sewage, hospital sewage, industrial wastewater) + sediment + activated sludge.

**③ Monitoring parameters (by medium — classification is commonly tested)**
- Surface-water basic items: water temperature, pH, DO, permanganate index, COD, BOD₅, ammonia-N, total N (lakes/reservoirs), total P, Cu/Zn/Se/As/Hg/Cd/Pb, hexavalent chromium, fluoride, cyanide, sulfide, volatile phenol, petroleum, anionic surfactant, fecal coliforms.
- Groundwater: required items (pH, total hardness, TDS, ammonia-N, nitrate-N, nitrite-N, volatile phenol, total cyanide, permanganate index, fluoride, As/Hg/Cd/hexavalent Cr/Fe/Mn, coliforms) + optional items.
- Wastewater: **Class I pollutants** (sampled at the workshop or workshop-treatment-facility outlet: total Hg, alkyl mercury, total Cd, total Cr, hexavalent Cr, total As, total Pb, total Ni, benzo(a)pyrene, total Be, total Ag, total α/total β radioactivity); **Class II pollutants** (sampled at the discharge unit's outlet: pH, color, suspended solids, BOD, COD, petroleum, animal/vegetable oil, volatile phenol, total cyanide, sulfide, ammonia-N, fluoride, phosphate, formaldehyde, anilines, nitrobenzenes, anionic surfactant, total Cu/Zn/Mn).
- 🔑 **The essential difference between Class I and Class II = sampling location:** Class I is highly toxic and must be controlled "at the source" (workshop outlet); Class II is controlled at the factory's main outlet.

**④ Layout & sampling** (details in Part 3 §3.1, §3.2)
- River cross-sections: background, **reference, control, reduction** (a single reach needs only the last three).
- Lakes/reservoirs: generally set monitoring verticals; use a grid where there is no obvious functional zoning.
- Sampling points on a vertical are set by water depth (see §3.1).
- Sampling frequency: drinking-water source ≥ once/month; rivers once/month, ≥ 6 times/year (high/low/normal-flow periods, ×2 each); national-controlled sections on days 5–10 of each month.

**⑤ Technique & instrument** (details in Part 2)
- Inorganic: chemical methods (gravimetry, titrimetry), AAS, spectrophotometry, ICP-OES, electrochemistry, ion chromatography, AFS, ICP-MS, gas-phase molecular absorption.
- Organic: GC, HPLC, GC-MS.

**⑥ Result & evaluation:** compare against GB3838 and similar standards; total discharge = average concentration over a period × wastewater discharge volume over that period.

---

## 1.2 Air & Waste-Gas Monitoring (Chapter 3)

**① Monitoring objectives:** grasp the current status and trends of ambient air quality; provide a basis for source management, emergency response, standard-setting, and research.

**② Monitoring targets**
- Ambient air (including indoor air).
- Pollution sources: stationary sources (stack/flue exhaust), mobile sources (vehicle exhaust).
- Precipitation (acid-rain monitoring).

**③ Parameters & pollutant classification (high-frequency)**
- By formation: **primary pollutants** (directly emitted from sources, physicochemical nature unchanged: SO₂, CO, NOₓ, particulates, benzo(a)pyrene); **secondary pollutants** (new pollutants formed by reactions among primary pollutants or with air components: O₃, aldehydes, PAN, sulfuric-acid mist, nitric-acid mist — mostly aerosols, often more toxic).
- By state of existence: **molecular state** (SO₂, CO, NOₓ, HCN, benzene, Hg, NH₃, H₂S, Pb, Cd, fluorides, etc.); **particulate state** (dustfall > 100 μm; TSP < 100 μm; PM₁₀ < 10 μm, inhalable; PM2.5 < 2.5 μm).

**④ Layout & sampling** (details in §3.1, §3.3)
- Layout principle: no pollution source within 50 m around; the sampling inlet should have ≥ 270° of collection space horizontally.
- Layout methods: functional-zone layout; **grid layout** (multiple uniform sources; 60% on the downwind side); **concentric-circle layout** (a cluster of sources); **sector (fan) layout** (an isolated elevated point source, angle ≤ 90°, commonly 45°).
- Sampling methods: **direct sampling** (high concentration: syringe, plastic bag, gas-sampling tube, evacuated bottle); **enrichment sampling** (low concentration 10⁻⁹–10⁻⁶: solution absorption, packed-column retention, filter-media retention, cryogenic condensation, electrostatic precipitation, diffusion/permeation, natural accumulation).

**⑤ Technique & instrument:** spectrophotometry (SO₂, NOₓ, etc.), GC (CO, hydrocarbons), NDIR (CO), chemiluminescence, gravimetry (TSP, PM₁₀, dustfall, sulfation rate).

**⑥ Result & evaluation:** Air Quality Index **AQI** (the maximum of the individual pollutant sub-indices IAQI); the primary pollutant = the one with the largest IAQI when AQI > 50.

---

## 1.3 Solid-Waste Monitoring (Chapter 4)

**① Monitoring objectives:** ① identify whether it is hazardous waste; ② provide a basis for treatment/disposal (landfill, incineration); ③ supervise the effectiveness of pollution control.

**② Monitoring targets:** industrial solid waste, **hazardous waste**, municipal refuse, medical waste, leachate.

**③ Parameters — "characteristic identification" of hazardous waste (core exam point)**
Hazardous waste = listed in the *National Catalogue of Hazardous Wastes* OR identified as having one of the following characteristics:

| Characteristic | Key criterion |
|---|---|
| **Flammability** | Liquid flash point < 60 °C; solid that can self-ignite by friction/moisture absorption |
| **Corrosivity** | Leachate pH ≤ 2 or ≥ 12.5; corrosion of steel > 0.64 cm/a (≤ 55.7 °C) |
| **Reactivity** | Violent change without detonation; reacts violently with water / forms explosive mixtures / releases toxic gas; explodes on heating or initiation |
| **Radioactivity** | Natural radioactivity specific activity > 3700 Bq/kg |
| **Acute toxicity** | Kills more than half of test mice within 48 h (LD₅₀ test) |
| **Leaching toxicity** | Leached by the prescribed method; harmful components in leachate exceed identification standards (see leaching-toxicity table in §3.4) |

**④ Layout & sampling** (details in §3.1)
- Number of increments: look up by batch size (e.g., batch 100–500 t → at least 20 increments).
- Increment mass: depends on the largest particle size (larger size → larger minimum increment mass).
- Layout: for stored/transported waste use diagonal, plum-blossom, checkerboard, S-shape; for a transport truck/container sample at three layers — top (1/6), middle (1/2), bottom (5/6).
- Sample preparation: crush → sieve → reduce by the **quartering method**; air-dry wet samples at room temperature.

**⑤ Technique & instrument:** leaching test + water-analysis methods; LD₅₀ animal test; calorific value by calorimeter; pH meter; corrosivity by glass-electrode method.

**⑥ Result & evaluation:** report on a dry-sample basis; use mg/kg when a pollutant is < 0.1%, and percent when > 0.1%.

---

## 1.4 Soil Quality Monitoring (Chapter 5)

**① Monitoring objectives:** ① soil-quality status monitoring; ② soil-pollution-accident monitoring; ③ dynamic monitoring of land treatment of pollutants; ④ soil background-value survey.

**② Monitoring targets:** farmland soil, contaminated-site soil (background value vs. polluted area).

**③ Monitoring parameters:** metal compounds, non-metallic inorganics, organic compounds (BHC, DDT, benzo(a)pyrene, etc.). The "yardstick" for judging pollution = the **soil background value** (the content of an element in soil under little or no human influence).

**④ Layout & sampling** (details in §3.1)
- Principle: lay out points wherever there is pollution; do not place points at field edges, ditch edges, roadsides, near fertilizer piles, or where there is erosion/topsoil disturbance.
- Number of points: at least 3 per unit; n = (s·t/d)² (t = 1.96 @ 95%, d = 0.2 @ 80% precision).
- Layout methods: **diagonal** (small plot, sewage irrigation; midpoints of 3–5 equal divisions of the diagonal), **plum-blossom** (small and uniform, 5–10 points), **checkerboard** (medium; > 10 points; **solid-waste-polluted soil > 20 points**), **S-shape** (large and non-uniform), **radial** (air-pollution type), **grid** (background value / agrochemical pollution).
- Sample types: **composite sample** (to check pollution status; 0–20 cm plow layer, orchard 0–60 cm; quartering method); **profile sample** (to check pollution depth; sampled by A/B/C horizons; profile 1.5 × 0.8 × 1.0 m; sampled from bottom upward).
- For heavy-metal samples, use bamboo trowels/strips where possible (to avoid metal contamination).

**⑤ Technique & instrument:** digestion (mixed acid / alkali fusion / pressurized vessel / microwave); AAS, ICP; GC (organochlorine pesticides, BaP); XRF (direct measurement of solids).

**⑥ Result & evaluation:** single-factor pollution index = measured value / standard value; integrated (Nemerow) pollution index = √[(mean single² + max single²)/2]; classified into 5 grades by the integrated index (≤ 0.7 safe … > 3.0 severe pollution).

---

## 1.5 Physical-Pollution Monitoring (Chapter 7: noise / vibration / radioactivity / light)

**① Monitoring objectives:** evaluate the impact of physical factors — sound, vibration, radiation, light — on the environment and the human body.

**② Monitoring targets & signature quantities**

| Sub-domain | Target | Signature quantity / unit |
|---|---|---|
| Noise | Urban/industrial/traffic noise | Sound pressure level Lp (dB), equivalent continuous A-level Leq |
| Vibration | Vibration sources | Vibration level |
| Radioactivity | α/β/γ radiation, electromagnetic radiation | Radioactivity (Bq), exposure (C/kg), absorbed dose (Gy), dose equivalent (Sv) |
| Light pollution | White-glare pollution, colored-light pollution | Illuminance, etc. |

**③–⑥ Noise as the main thread (most commonly tested)**
- Physical quantities: sound power W (W), sound intensity I (W/m²), sound pressure p (Pa); the corresponding "levels": Lw, LI, Lp.
- Subjective–objective relation: loudness (sone), loudness level (phon), weighted sound level (A-weighting is most common, simulating the human ear).
- Evaluation quantities: equivalent continuous A-level Leq, day–night equivalent level Ldn.
- Instrument: sound level meter (measures sound pressure level with frequency weighting + time weighting).
- Calculations: sound pressure level, noise addition/subtraction, Leq (see §3.4).

**Radioactivity essentials:** α decay (heavy nuclei Z > 82 emit ⁴He), β decay (emits electrons; includes β⁻/β⁺/electron capture), γ decay (electromagnetic radiation); half-life T₁/₂; exposure X = dQ/dm, absorbed dose D = dε/dm, dose equivalent H = D·Q·N.

---

# Part 2　Overview of Instruments & Analytical Techniques (Horizontal Integration)

> The course scatters the various instruments/methods across the water, air, soil, and solid-waste chapters. This part **groups them by technique family** and gives two "two-way lookup" master tables: ① method → what it measures; ② pollutant → which method to use. This is the core weapon for "method–pollutant pairing" questions.

## 2.1 The five technique families (build the big categories first)

| Family | Representative methods | Core principle in one line |
|---|---|---|
| **Spectrometry** | Spectrophotometry, AAS, AFS, ICP-OES/AES, ICP-MS, gas-phase molecular absorption | A substance's absorption/emission/fluorescence of light correlates with concentration |
| **Chromatography** | GC, HPLC, ion chromatography (IC), GC-MS, headspace/purge-and-trap | Separation by differences in partition coefficient between stationary/mobile phases |
| **Electrochemistry** | Potentiometry (ion-selective electrode, pH, oxygen electrode), anodic stripping voltammetry, coulometric titration, conductivity | Measure potential/current/charge/conductivity vs. concentration |
| **Titrimetry/Gravimetry** | Iodometry, dichromate method, silver-nitrate titration, gravimetry | Classical stoichiometric reactions |
| **Biological** | BOD incubation, microbial electrode, toxicity test | Use the response of microbes/organisms to pollutants |

## 2.2 "Principle + what it measures + features" quick memory for each method

**Spectrometry**
- **Spectrophotometry** (UV/visible/IR): based on molecular absorption spectra; quantification follows the **Beer–Lambert law A = Kbc**. Convert the analyte to a colored species and measure absorbance at the characteristic wavelength. Cheap, ubiquitous, the workhorse of routine monitoring. Wavelength regions: UV 10–400 nm, visible 400–780 nm, IR 780 nm–300 μm.
  - Dithizone spectrophotometry: measures Hg, Pb, Cd, Zn, etc. (forms colored chelates).
- **Atomic Absorption Spectrometry (AAS):** absorption of an element's characteristic resonance radiation by its atomic vapor; flame/graphite-furnace atomizes the sample into ground-state atoms, then absorbance is measured. Cold-vapor atomic absorption (253.7 nm, SnCl₂ reduction) is dedicated to mercury. Mainly for trace/ultratrace metals.
- **Atomic Fluorescence Spectrometry (AFS):** cold-vapor atomic fluorescence for Hg, etc.
- **ICP-OES/AES** (inductively coupled plasma optical/atomic emission spectrometry): plasma torch at 6000–8000 K; atoms are excited and emit characteristic spectra; **I = aC^b**. High accuracy, low detection limits, wide linear range, **simultaneous multi-element determination**.
- **ICP-MS:** detection by mass-to-charge ratio; trace multi-element.
- **Gas-phase molecular absorption spectrometry:** measures ammonia-N, nitrate-N, nitrite-N, sulfide, etc.

**Chromatography**
- **Gas Chromatography (GC):** separates volatile, thermally stable organics. **Detectors (high-frequency exam point):**
  - **FID (flame ionization):** destructive, mass-type, universal, high sensitivity, wide linearity; measures only organics (carbon-containing); **cannot measure inert gases / air / water / CO / CO₂ / CS₂ / NO / SO₂ / H₂S**.
  - **ECD (electron capture):** β radioactive source; highly selective, responds only to electron-capturing compounds (halogenated hydrocarbons, N/O/S-containing); measures trace pesticides, PCBs.
  - **TCD (thermal conductivity):** universal, non-destructive, concentration-type; low sensitivity → macro-quantity analysis.
  - **FPD (flame photometric):** mass-type, selective; dedicated to **S, P** compounds (hydrogen-rich flame; S characteristic 394 nm, P characteristic 526 nm).
- **Ion Chromatography (IC):** continuous determination of multiple ions (anions such as fluoride, chloride).
- **HPLC:** high-boiling, thermally unstable, large-molecule compounds (e.g., PAHs, benzo(a)pyrene).
- **GC-MS:** both qualitative and quantitative; trace organics, PAHs, VOCs.
- **Headspace GC / purge-and-trap GC:** pretreatment + determination of volatile halogenated hydrocarbons, VOCs.

**Electrochemistry**
- **Potentiometry (ion-selective electrode):** F⁻ (fluoride ISE), pH (glass electrode).
- **Oxygen-electrode method (Clark electrode):** measures DO, I = KC.
- **Anodic stripping voltammetry:** measures trace heavy metals (Cd, Pb, Cu, Zn, etc.).
- **Coulometric titration:** measures COD, SO₂; based on Faraday's law W = ItM/(96500n).
- **Conductivity:** measures mineralization, precipitation conductivity.

**Titrimetry/Gravimetry**
- **Iodometry:** measures DO (modified iodometry removes nitrite/ferrous interference).
- **Dichromate method:** measures COD (classic).
- **Silver-nitrate titration:** measures cyanide, chloride.
- **Gravimetry:** measures TSP, PM₁₀, dustfall, sulfation rate (lead dioxide / alkali plate), mineralization, soluble salts, oils.

**Biological methods**
- **BOD 5-day incubation:** measures BOD₅.
- **Microbial-electrode method:** rapid BOD measurement.
- **Toxicity test (LD₅₀):** acute-toxicity identification of hazardous waste.

## 2.3 ⭐ Master Table A: Method → Principle → Applicable Pollutants → Features

| Method | Principle keyword | Main applicable pollutants | Features |
|---|---|---|---|
| Spectrophotometry | Beer–Lambert A = Kbc | Ammonia-N, total P, phenol, sulfide, cyanide, SO₂, NOₓ, many metals | Cheap & ubiquitous, workhorse of routine monitoring |
| Dithizone spectrophotometry | Colored chelate | Hg, Pb, Cd, Zn | Color development, light-protected, high purity needed |
| AAS (flame/graphite furnace) | Ground-state atoms absorb characteristic radiation | Many trace/ultratrace metals (Pb, Cd, Cu, Zn, Cr…) | Sensitive, element-specific |
| Cold-vapor AAS/AFS | Hg is volatile, SnCl₂ reduction | **Mercury** (253.7 nm) | Dedicated to Hg |
| ICP-OES/AES | Plasma-torch excitation & emission | Many metals/metalloids (Al, Fe, Cd, Cr, As…) | Simultaneous multi-element, low detection limit |
| Ion chromatography (IC) | Ionic partition separation | Fluoride, chloride, sulfate, nitrate, and other anions | Multiple ions in one run |
| GC (FID/ECD/FPD/TCD) | Partition-coefficient difference | Volatile halogenated hydrocarbons, VOCs, pesticides, hydrocarbons, CO | Selectivity depends on detector |
| HPLC | Liquid-phase partition | PAHs, benzo(a)pyrene | High-boiling, non-volatile substances |
| GC-MS | Mass-to-charge ratio | PAHs, VOCs, specific organics | Qualitative & quantitative |
| Ion-selective electrode | Potential | F⁻, pH | Direct, fast |
| Oxygen-electrode method | Diffusion current | Dissolved oxygen DO | On-site continuous |
| Anodic stripping voltammetry | Enrichment-stripping | Trace heavy metals | Sensitive |
| Iodometry | I₂ titration | Dissolved oxygen DO | Classic |
| Dichromate method | Strong oxidant | COD | Classic, oxidation rate ≈ 90% |
| Coulometric titration | Faradaic electrolysis | COD, SO₂ | Instrumentalized |
| Gravimetry | Weight difference | TSP, PM₁₀, dustfall, sulfation rate, mineralization, oils | Direct but time-consuming |
| BOD incubation / microbial electrode | Microbial oxygen uptake | BOD | Reflects biodegradability |

## 2.4 ⭐ Master Table B: Pollutant → Available Methods (reverse lookup)

| Pollutant | Available methods (⭐ = representative/most classic) |
|---|---|
| **Mercury (Hg)** | ⭐Cold-vapor AAS (253.7 nm), cold-vapor AFS, dithizone spectrophotometry, anodic stripping voltammetry, potentiometry |
| **Cadmium (Cd)** | ⭐AAS, dithizone spectrophotometry, anodic stripping voltammetry, ICP-OES |
| **Lead (Pb)** | AAS, dithizone spectrophotometry, anodic stripping voltammetry, ICP-OES, oscillographic polarography |
| **Copper (Cu) / Zinc (Zn)** | AAS, dithizone spectrophotometry, ICP-OES |
| **Chromium (Cr)** | ⭐Diphenylcarbazide spectrophotometry (hexavalent Cr), flame AAS (total Cr), ICP-OES, ferrous-ammonium-sulfate titration |
| **Arsenic (As)** | New silver-salt spectrophotometry, hydride-generation AAS, ICP-OES |
| **Aluminum (Al)** | ICP-OES, indirect flame AAS, spectrophotometry |
| **Dissolved oxygen (DO)** | ⭐Iodometry, modified iodometry (sodium azide / permanganate), oxygen-electrode method |
| **COD** | ⭐Dichromate method, coulometric titration, rapid sealed-digestion titration/photometry, chlorine-correction method |
| **Permanganate index** | KMnO₄ oxidation (acidic/alkaline) |
| **BOD** | ⭐5-day incubation, microbial-electrode method |
| **TOC** | Combustion-oxidation NDIR method (TC − IC = TOC) |
| **Ammonia-N** | Nessler's-reagent spectrophotometry, distillation–neutralization titration, gas-phase molecular absorption, electrode method |
| **Cyanide** | ⭐Isonicotinic-acid–pyrazolone / pyridine–barbituric-acid spectrophotometry, silver-nitrate titration |
| **Fluoride** | ⭐Ion-selective-electrode method, ion chromatography, fluoride-reagent spectrophotometry |
| **Sulfide** | Indirect flame AAS, gas-phase molecular absorption, methylene-blue spectrophotometry |
| **Total P / phosphate** | Ammonium-molybdate spectrophotometry |
| **Volatile phenol** | 4-aminoantipyrine spectrophotometry, bromination titration (high concentration), chromatography |
| **Nitrobenzenes** | Reduction–azo spectrophotometry (mono/di-nitro), chlorinated-cetylpyridine spectrophotometry (tri-nitro) |
| **Oils** | Gravimetry, IR spectrophotometry, NDIR |
| **Volatile halogenated hydrocarbons** | Headspace GC (ECD), GC-MS |
| **VOCs** | Purge-and-trap GC, headspace GC-MS |
| **PAHs / benzo(a)pyrene** | HPLC, GC-MS, fluorescence spectrometry, paper/thin-layer chromatography |
| **SO₂ (air)** | ⭐Formaldehyde-absorption–pararosaniline spectrophotometry (577 nm), tetrachloromercurate method, thorin method, constant-potential electrolysis |
| **NOₓ (air)** | ⭐N-(1-naphthyl)ethylenediamine spectrophotometry (540 nm), acidic-permanganate oxidation, coulometric titration |
| **CO (air)** | ⭐NDIR method, GC, constant-potential electrolysis, mercury-displacement method |
| **O₃ / photochemical oxidants** | Boric-acid–potassium-iodide spectrophotometry, chemiluminescence |
| **Fluoride (air)** | Filter/lime-paper sampling — ion-selective-electrode method |
| **TSP / PM₁₀** | Gravimetry (high/medium/low-volume sampling), piezoelectric crystal, light scattering |
| **Sulfation rate** | Lead-dioxide gravimetry, alkali-plate gravimetry, alkali-plate ion chromatography |
| **Soil organochlorine pesticides (BHC/DDT)** | GC (ECD) |

## 2.5 Signature data for quick memory (commonly tested in fill-in/multiple-choice)

| Item | Value |
|---|---|
| Beer–Lambert law | A = lg(1/T) = Kbc; A ∝ c, A ∝ b |
| Visible-light wavelength | 400–780 nm |
| Cold-vapor AAS Hg wavelength | 253.7 nm |
| SO₂ formaldehyde–pararosaniline max absorption | 577 nm |
| NOₓ N-(1-naphthyl)ethylenediamine wavelength | 540 nm |
| FPD S/P characteristic wavelength | S 394 nm / P 526 nm |
| ICP torch temperature | 6000–8000 K |
| Reference sound pressure p₀ | 2 × 10⁻⁵ Pa |
| Reference sound power W₀ / intensity I₀ | 10⁻¹² W / 10⁻¹² W·m⁻² |
| Dichromate / permanganate oxidation rate | ≈ 90% / ≈ 50% |
| TOC combustion temperature | High-temp furnace 900–950 °C, low-temp furnace 150 °C |
| Dry-ashing temperature | 450–550 °C |

---

# Part 3　Key Procedures, Site Layout & Calculations in Detail (with worked examples)

## 3.1 Big comparison of layout schemes (you must be able to distinguish these)

### 3.1.1 Water — river monitoring cross-sections (most commonly tested)

| Cross-section | Location | Function |
|---|---|---|
| **Background (背景)** | A reach essentially unaffected by human activity | The "baseline" for evaluating pollution of the whole water system |
| **Reference / upstream (对照)** | Before entering the monitored reach (generally only 1 per reach) | Reflects the inflow baseline water quality of the reach |
| **Control / impact (控制)** | Downstream of the discharge area (outlet), where sewage and river water are essentially mixed (number set by industrial layout and outlets) | Reflects the impact of pollution sources on the water body |
| **Reduction (削减)** | **More than 1500 m downstream of the last outlet** of the city/industrial area | Reflects the situation where pollutants are markedly reduced after dilution, dispersion, and self-purification |

> Mnemonic: "**background–reference–control–reduction**"; the concentration trend is baseline → inflow → most heavily polluted → reduced by self-purification. A complete water system sets all four; a single reach needs only "reference, control, reduction."

**Determining sampling points on a vertical (by water depth — commonly tested)**

| Water depth | Sampling points |
|---|---|
| < 5 m | 1 point, 0.5 m below the surface |
| 5–10 m | 2 points: 0.5 m below surface, and 0.5 m above the bottom |
| > 10 m | 3 points: 0.5 m below surface, at ½ depth, and 0.5 m above the bottom |

Lakes/reservoirs: generally set only monitoring verticals; with no obvious functional zoning, use the **grid method** for uniform layout; for heavily polluted lakes/reservoirs, set control sections along the main pollutant-transport routes.
Groundwater: two well types — **background monitoring wells** (in unpolluted ground, upstream of groundwater flow, perpendicular to flow direction) and **pollution-control monitoring wells** (around the source, especially downstream).

### 3.1.2 Air — comparison of the three layout methods

| Layout method | Applicable situation | Key points |
|---|---|---|
| **Functional-zone** | Routine regional monitoring | Divide into industrial/commercial/residential/traffic/clean zones, set several points each; no averaging required |
| **Grid** | Multiple uniformly distributed sources | More points downwind of the prevailing wind, accounting for **60%** of the total |
| **Concentric-circle** | A pollution cluster of multiple sources | Draw concentric circles centered on the cluster's center, place points on the circles, more downwind |
| **Sector (fan)** | An isolated elevated point source with a clear prevailing wind | Point source as apex, prevailing wind as axis; angle usually 45°, **≤ 90°**; 3–4 points per arc; set a reference point upwind |

Supplement: location of the maximum ground-level concentration from a tall stack (50 m) — unstable conditions 5–10 × stack height, neutral ≈ 20 ×, stable ≥ 40 ×.

### 3.1.3 Soil — the six layout methods

Diagonal (small sewage-irrigated plot; midpoints of 3–5 equal divisions of the diagonal), plum-blossom (small and uniform, 5–10 points), checkerboard (medium, > 10 points; **solid-waste-polluted soil > 20 points**), S-shape (large and non-uniform), radial (air-pollution type; draw rays from the source, denser downwind), grid (background value / agrochemical pollution).

### 3.1.4 Solid waste — increment count and sampling points

- Number of increments by batch lookup (larger batch → more increments, e.g., 1000–5000 t → 30 increments).
- Increment mass by the largest particle size (larger size → larger minimum increment mass, e.g., > 150 mm → 30 kg).
- Stored/transported waste: diagonal, plum-blossom, checkerboard, S-shape.
- Transport truck/container: top (1/6 depth below surface), middle (1/2 depth), bottom (5/6 depth).
- Sample preparation: crush → sieve → **reduce by quartering**.

## 3.2 Sampling, preservation, and precautions

### 3.2.1 Water-sample types (easily confused)

| Type | Time | Location | Notes / applicability |
|---|---|---|---|
| Grab sample | One time | One location | When water quality is stable; one-off sampling |
| **Composite (综合)** | **Simultaneous** | **Different points** | Collected simultaneously at different points then mixed (e.g., a combined treatment plant built for several discharge channels) |
| **Mixed (混合)** | **Different times** | **Same point** | Same point, mixed at equal-time/equal-proportion over different times (a source with constant flow but varying quality) |
| Average sewage sample | Periodic | Same/different points | A source with both varying flow and quality (suitable for domestic sewage) |
| Average proportional mix | Different/same times | Same/different points | Mixed proportionally when discharge is unstable |

> Distinguishing rule: **composite = simultaneous, different points; mixed = same point, different times.**

### 3.2.2 Water-sample preservation methods (high-frequency)

Four basic means:
1. **Refrigeration/freezing:** inhibit microbes, slow volatilization and reactions. Refrigerate 2–5 °C (not long-term); freeze −20 °C (do not fill the container completely).
2. **Add biological inhibitor:** e.g., add HgCl₂ to preserve phosphate.
3. **Adjust pH:** for metal ions add HNO₃ to **pH 1–2** (prevent hydrolysis/precipitation + prevent wall adsorption); for cyanide/volatile phenol add NaOH to **pH 12** to form stable salts.
4. **Add oxidant/reductant:** for mercury add HNO₃ (pH < 1) + 0.05% K₂Cr₂O₇ (keep high valence); for sulfide add ascorbic acid (prevent oxidation); for DO add manganese sulfate + alkaline potassium iodide (fixation).

Containers and stoppers: alkaline samples cannot use glass stoppers → use rubber stoppers; organics/bacteria cannot use rubber stoppers. For dissolved fractions, first filter through a **0.45 μm membrane**.

Commonly tested preservation entries: COD — add H₂SO₄ to pH < 2, can keep 7 d; DO (iodometry) — add manganese sulfate + alkaline KI, 4–8 h (measure on-site); ammonia-N/nitrate — add H₂SO₄ to pH < 2, 24 h; hexavalent Cr — add NaOH to pH 8–9, measure the same day.

### 3.2.3 Sampling precautions (water)

Items requiring separate sampling: suspended solids, pH, DO, BOD, oils, sulfide, residual chlorine, radioactivity, microbes. Must fill the container completely: DO, BOD, organics. Best measured on-site: pH, conductivity, DO. Sampling must be synchronized with hydrological and meteorological parameters; label sample bottles, seal tightly, and complete the sampling-registration form.

### 3.2.4 Pretreatment

**Digestion (for inorganic elements in organic-containing water samples)** — purpose: destroy organic matter, dissolve suspended solids, and oxidize the analyte to a single high-valence state. After digestion the solution should be clear and transparent with no precipitate.
- Wet methods: nitric acid (cleaner water), nitric–perchloric acid (hard-to-oxidize organics), **nitric–sulfuric acid (5:2)**, sulfuric–phosphoric acid (eliminate Fe³⁺ interference), **sulfuric acid–permanganate (for Hg)**, multi-component (for total Cr: sulfuric + phosphoric + permanganate), alkaline decomposition (prevent loss of volatile components).
- Dry ashing: ignite at 450–550 °C; **not applicable to volatile elements (As, Hg, Cd, Se, Sn)**.

**Enrichment and separation:** gas stripping (Hg, sulfide), headspace (VOCs), distillation, solvent extraction, solid-phase extraction (SPE), adsorption, ion exchange, coprecipitation, cryogenic concentration. For soil-organics extraction, shaking extraction and Soxhlet extraction (pesticides, benzo(a)pyrene) are common.

## 3.3 Evaluation standards & pollution-index system (result expression)

- Water: compare against GB3838-2002 *Surface Water Environmental Quality Standard*; total discharge = average concentration × discharge volume.
- Air: AQI (see §3.4.6).
- Soil: single-factor / integrated pollution index (see §3.4.9).
- Solid waste: compare leaching toxicity against identification standards.

---

## 3.4 ⭐ Key Calculation Topics (formula + example + solution)

> Calculation questions are decisive for spreading scores. Each topic below gives "formula + example + solution." It is recommended to mentally compute each one yourself.

### 3.4.1 Beer–Lambert law

$$A=\lg\frac{1}{T}=Kbc$$
A absorbance; T transmittance; K absorption coefficient; b path length (cm); c concentration. A is proportional to c and b.
**Usage:** standard-curve method — measure A vs. c for a series of standard solutions and plot, then read c from the sample's A.

### 3.4.2 Dissolved oxygen DO (iodometry)

Reaction chain (you should be able to write it):
```
MnSO₄ + 2NaOH → Mn(OH)₂↓
2Mn(OH)₂ + O₂ → 2MnO(OH)₂   (brown precipitate, "fixes" the dissolved oxygen)
MnO(OH)₂ + 2H₂SO₄ → Mn(SO₄)₂ + 3H₂O
Mn(SO₄)₂ + 2KI → MnSO₄ + I₂ + K₂SO₄
I₂ + 2Na₂S₂O₃ → 2NaI + Na₂S₄O₆   (titration with sodium thiosulfate)
```
- **Modified iodometry:** nitrite interference → **sodium-azide** method; Fe²⁺ interference → **permanganate** method.
- DO (mg/L) = (c·V·8 × 1000)/V_sample (c: Na₂S₂O₃ concentration mol/L; V: titration volume mL; 8 = oxygen equivalent).

### 3.4.3 COD (dichromate method)

$$COD_{Cr}(\text{mg O}_2/L)=\frac{(V_0-V_1)\times c\times 8\times1000}{V_{sample}}$$
- V₀: volume of ferrous ammonium sulfate consumed by the blank titration (mL); V₁: volume consumed by the sample (mL); c: ferrous-ammonium-sulfate concentration (mol/L); 8 = half the molar mass of oxygen (8 g O per electron transferred); V_sample: sample volume (mL).
- Reagent selection: COD > 50 use 0.25 mol/L K₂Cr₂O₇; COD 5–50 use 0.025 mol/L (lower accuracy).
- Interference: Cl⁻ is oxidized and interferes → add **mercuric sulfate** to complex/mask it; catalyst **silver sulfate**; indicator **ferroin (test-ferrous)**. Pyridine is not oxidized; aromatics are hard to oxidize.

**Example:** Take 20.0 mL of sample; after reflux, titrate with 0.250 mol/L ferrous ammonium sulfate; the blank consumes V₀ = 20.0 mL and the sample consumes V₁ = 12.0 mL. Find COD.
**Solution:** COD = (20.0 − 12.0) × 0.250 × 8 × 1000 / 20.0 = 8.0 × 0.250 × 8 × 1000 / 20.0 = **800 mg/L**.

### 3.4.4 Coulometric titration (Faraday's law)

$$W=\frac{I\,t\,M}{96500\,n}$$
W mass of substance reacted at the electrode; I electrolysis current; t time; M molar mass; n electrons transferred per mole; 96500 Faraday constant.

### 3.4.5 BOD (biochemical oxygen demand)

**Definition:** the DO consumed by aerobic microbes decomposing organic matter under dissolved-oxygen conditions (20 ± 1 °C, dark, 5 days = BOD₅).

**Theoretical-oxygen-demand example (balance the equation):** find the theoretical oxygen demand of 1.67 × 10⁻³ mol/L glucose.
C₆H₁₂O₆ + 6O₂ → 6CO₂ + 6H₂O
1.67 × 10⁻³ mol/L × 6 (mol O₂/mol glucose) × 32 (g/mol) = 0.321 g/L = **321 mg O₂/L**.

**5-day incubation calculations:**
- **Dilution water not seeded:** BOD₅ = (D₁ − D₂)/P
- **Dilution water seeded:** BOD₅ = [(D₁ − D₂) − (B₁ − B₂)·f] / P

D₁ DO of diluted sample before incubation; D₂ DO after 5 days; B₁, B₂ DO of the seeded control before/after; f = fraction of seeded dilution water in the total volume; P = fraction of sample in the total volume (P = sample volume / 300).

**Validity criterion:** valid only if the diluted sample's 5-day **oxygen uptake > 2 mg/L and residual DO > 1 (or 2) mg/L**; average the valid dilutions.

**Example (simplified "uptake × 300 / sample volume"):** a sample with two dilutions A, B:
| | A | B |
|---|---|---|
| Sample volume mL | 15 | 30 |
| Initial DO | 8.1 | 8.2 |
| 5-day DO | 5.6 | 3.3 |
| Oxygen uptake | 2.5 | 4.8 |
BOD_A = 2.5 × 300/15 = 50 mg/L; BOD_B = 4.8 × 300/30 = 48 mg/L; both valid → average = (50 + 48)/2 = **49 mg/L**.
(If a dilution's uptake < 2 or residual DO is insufficient, that dilution is invalid and discarded.)

**BOD reaction model (first-order kinetics):**
- Remaining organic matter (as oxygen equivalent): $L_t=L_0e^{-k_1t}$
- Already consumed (i.e., BOD at time t): $y_t=L_0(1-e^{-k_1t})$, where L₀ = ultimate (total) carbonaceous BOD (UBOD).
- k₁ values: untreated wastewater 0.12–0.46 d⁻¹ (typical 0.23); biologically treated effluent 0.12–0.23 d⁻¹.
- Temperature correction: $k_T=k_{20}\theta^{(T-20)}$, θ usually 1.047 (1.056 for 20–30 °C, 1.135 for 4–20 °C).

**Nitrification (NBOD):** NH₃ + 2O₂ → HNO₃ + H₂O; usually significant only from days 5–8, so BOD₅ generally **does not include the nitrification stage** (it is carbonaceous CBOD). The two stages = the carbon-oxidation stage + the nitrification stage.

**Dilution-water requirements:** prepared from distilled water, aerated 2–8 h to near-saturation DO, with CaCl₂/FeCl₃/MgSO₄ nutrients + phosphate buffer added, pH ≈ 7.2, its own BOD₅ < 0.2 mg/L; when there are no microbes, add a seed liquid (supernatant of domestic sewage, etc.). A glucose + glutamic-acid standard solution diluted 1:50 should give **180–230 mg/L**.

### 3.4.6 Air Quality Index AQI

**Sub-index IAQI** (linear interpolation):
$$IAQI_P=\frac{IAQI_{Hi}-IAQI_{Lo}}{BP_{Hi}-BP_{Lo}}(C_P-BP_{Lo})+IAQI_{Lo}$$
- C_P measured concentration of the pollutant; BP_Hi/BP_Lo the high/low concentration breakpoints adjacent to C_P; IAQI_Hi/IAQI_Lo the corresponding sub-indices.
**AQI = max{IAQI₁, IAQI₂, …}**; when AQI > 50, the one with the largest IAQI is the **primary pollutant**; any with IAQI > 100 is an **exceeding (over-standard) pollutant**.
Pollutants included: SO₂, NO₂, PM₁₀, CO (daily average) + O₃ (8-h average) (including PM2.5).

**Example:** at a site SO₂(24h) = 80 μg/m³, NO₂(24h) = 120 μg/m³, PM2.5(24h) = 150 μg/m³; find each IAQI, the AQI, and the primary pollutant.
**Solution (interpolating with the GB3095-2012 sub-index breakpoint table):**
- SO₂: 80 falls in [50,150) → IAQI = (100−50)/(150−50) × (80−50) + 50 = 50/100 × 30 + 50 = **65**.
- NO₂: 120 falls in [80,180) → IAQI = (100−50)/(180−80) × (120−80) + 50 = 50/100 × 40 + 50 = **70**.
- PM2.5: 150 falls in [115,150] → IAQI = (200−150)/(150−115) × (150−115) + 150 = 50 + 150 = **200**.
- AQI = max{65, 70, 200} = **200**, primary pollutant = **PM2.5** (and IAQI > 100, so it is an exceeding pollutant).
> Note: breakpoints follow the current GB3095-2012 table; the method is unchanged — "locate the interval → linear interpolation → take the maximum."

### 3.4.7 Sound pressure level & noise addition/subtraction (high-frequency calculation)

**The three "levels"** (memorize the reference quantities):
$$L_W=10\lg\frac{W}{W_0}\quad(W_0=10^{-12}\,W)$$
$$L_I=10\lg\frac{I}{I_0}\quad(I_0=10^{-12}\,W/m^2)$$
$$L_p=10\lg\frac{p^2}{p_0^2}=20\lg\frac{p}{p_0}\quad(p_0=2\times10^{-5}\,Pa)$$

**Noise addition:** sound energy/intensity can be added algebraically; **sound pressure cannot be added directly**. Total sound pressure level:
$$L_{p,total}=10\lg\!\left(10^{L_{p1}/10}+10^{L_{p2}/10}\right)$$
In engineering, use the "increment curve": from the level difference ΔL, look up ΔLp and add it to the larger level.
- **Example:** L_p1 = 96 dB, L_p2 = 93 dB, difference 3 dB → from the curve ΔLp ≈ 1.8 dB → L_p,total = 96 + 1.8 = **97.8 dB**.
- Multiple sources: add pairwise in succession; the order does not matter.

**Noise subtraction (removing background):** with measured-plus-background L_p and background L_p1, the difference ΔL = L_p − L_p1 gives ΔLp from the background-correction curve; the machine's actual level L_p2 = L_p − ΔLp.
- **Example:** measured 104 dB, background 100 dB, difference 4 dB → ΔLp ≈ 2.2 dB → machine's actual level = 104 − 2.2 = **101.8 dB**.

### 3.4.8 Equivalent continuous A-level Leq

$$L_{eq}=10\lg\!\left(\frac{1}{T}\int_0^T 10^{0.1L_{pA}}\,dt\right)$$
Discrete form (each level L_i occupies time fraction t_i/T):
$$L_{eq}=10\lg\!\left(\frac{1}{N}\sum_i 10^{0.1L_i}\right)\ (\text{equal time intervals})$$
**Example:** three equal-time segments measured at 60, 60, 70 dB; Leq = 10·lg[(10⁶ + 10⁶ + 10⁷)/3] = 10·lg[(1.2 × 10⁷)/3] = 10·lg(4 × 10⁶) ≈ **66.0 dB** (note this is an energy average, biased toward the larger values relative to an arithmetic mean).

### 3.4.9 Soil pollution index

- Single-factor pollution index: $P_i=\dfrac{C_i(\text{measured})}{S_i(\text{standard})}$
- Integrated (Nemerow) pollution index: $P_{int}=\sqrt{\dfrac{\bar P^2+P_{max}^2}{2}}$ ($\bar P$ is the mean of the single-factor indices, $P_{max}$ the maximum single-factor index).
- Classification: P_int ≤ 0.7 safe (clean); 0.7–1.0 alert (still clean); 1.0–2.0 slight pollution; 2.0–3.0 moderate/heavy pollution; > 3.0 severe pollution.
- Exceedance multiple = (measured − standard)/standard; share ratio = a factor's index / the sum of all indices.

### 3.4.10 Solid-waste calorific-value conversion

High calorific value H₀ → low calorific value Hₙ (subtracting energy for water vapor and heating moisture):
$$H_n=H_0\times\frac{100-(w_1+W)}{100}-5.85\,W_L$$
(w₁ inert-matter content %, W surface moisture %, W_L residual and hygroscopic moisture %). An important incineration indicator; refuse incineration can generate electricity.

### 3.4.11 Standard-gas preparation

- **Static preparation:** a metered amount of source gas is added to a vessel of known volume, then diluent gas is added; concentration is computed from the added amount and the volume. Example: a 100 mL syringe draws 99.99% CO; diluting 10× each time for 6 successive times → 1 × 10⁻⁶. Simple, but reactive gases are easily adsorbed/reacted at the walls.
- **Dynamic preparation:** continuous-dilution method, negative-pressure injection method, permeation-tube method, gas-diffusion method, electrolysis method. The permeation-tube method can be quantified by gravimetry or chemical analysis.

### 3.4.12 Radioactivity-related

- Half-life T₁/₂: the time for a radionuclide to decay to half its original amount.
- Exposure X = dQ/dm (C/kg, old unit roentgen R).
- Absorbed dose D = dε/dm (J/kg, gray Gy).
- Dose equivalent H = D·Q·N (Q quality factor; unit Sv).

### 3.4.13 Two ways of expressing air concentration and their conversion

- Mass concentration (mg/m³): applicable to any state.
- Volume fraction (mL/m³): only for gaseous/vapor states; independent of T and P.
- Conversion (STP): mass concentration = volume fraction × M / 22.4 (then correct for actual T, P).

### 3.4.14 Activated sludge (SV, SVI)

- Sludge settling ratio SV₃₀ (%): pour the mixed liquor into a 1000 mL cylinder, let it settle for 30 min; settled-sludge volume / mixed-liquor volume.
- Sludge volume index SVI = SV₃₀ (mL/L) ÷ MLSS (g/L) (i.e., the volume in mL occupied by 1 g of dry sludge after settling).

---

# Part 4　Core Concepts, Standards & Cases

## 4.1 Must-memorize list of term definitions (ranked by probability)

- **Environmental monitoring:** the activity of measuring the types, concentrations, distribution, and trends of pollutants in the environment in order to judge environmental quality.
- **Water body:** the collective term for surface water, groundwater, and the sediment, aquatic organisms, etc., they contain (note: not just "water").
- **Chemical oxygen demand (COD):** the amount of oxidant consumed in oxidizing reducing substances in 1 L of water sample under specified conditions, expressed as mg/L of O₂.
- **Biochemical oxygen demand (BOD):** the dissolved oxygen consumed in the biochemical oxidation process by which aerobic microbes decompose organic matter in water under dissolved-oxygen conditions.
- **Permanganate index:** the chemical oxygen demand measured using KMnO₄ as the oxidant; reflects the degree of pollution of surface water by organic matter and reducing inorganics.
- **Total organic carbon (TOC):** a comprehensive indicator expressing the total amount of organic matter in water by its carbon content (combustion method; reflects total organics better than BOD/COD).
- **Dissolved oxygen (DO):** molecular oxygen dissolved in water.
- **Primary / secondary pollutant:** see §1.2.
- **Photochemical smog:** a mixture of pollutants formed by the reaction of nitrogen oxides and hydrocarbons under ultraviolet light; the most destructive are O₃ and PAN.
- **Water eutrophication:** the phenomenon in which excess nutrients such as N and P in a water body cause excessive algal growth and water-quality deterioration.
- **Hazardous waste:** solid waste listed in the national catalogue of hazardous wastes or identified as having hazardous characteristics such as flammability, corrosivity, reactivity, or toxicity.
- **Leaching toxicity:** the hazardous characteristic in which, after leaching by the prescribed method, the concentration of harmful components in the leachate exceeds the identification standard.
- **Soil background value (baseline value):** the content of an element in soil under little or no human influence; the yardstick for judging whether soil is polluted.
- **Sound pressure level Lp:** ten times the logarithm of the ratio of sound-pressure squared to reference-sound-pressure squared (= 20 lg(p/p₀)), in dB.
- **Equivalent continuous sound level Leq:** the continuous steady A-level with equal sound energy over the same time period, representing the noise magnitude of that period.
- **Half-life T₁/₂:** the time for a radionuclide to decrease to half its original amount through decay.
- **Air Quality Index (AQI):** an index that simplifies the concentrations of the main routinely monitored pollutants into a single value and classifies air quality (takes the maximum of the sub-indices).
- **Grab / mixed / composite water samples:** see §3.2.1.

## 4.2 Important standard numbers (memorize the key few)

| Standard No. | Name |
|---|---|
| GB3838-2002 | Surface Water Environmental Quality Standard |
| GB3097-1997 | Seawater Quality Standard |
| GB5084-2021 | Farmland Irrigation Water Quality Standard |
| HJ164-2020 | Technical Specifications for Groundwater Environmental Monitoring |
| GB/T11914-1989 | Water Quality — Determination of COD — Dichromate Method |
| HJ505-2009 | Water Quality — Determination of BOD₅ (5-day Incubation) |
| GB3095 (-2012) | Ambient Air Quality Standard (basis for AQI; the 1996 version is used for API) |
| GB15618-1995 | Soil Environmental Quality Standard |
| GB5085 | Identification Standards for Hazardous Waste (series) |
| GB3096 | Acoustic Environment Quality Standard |
| HJ/T92-2002 | Technical Specifications for Total-Amount Monitoring of Water Pollutants |

## 4.3 Classic pollution events (commonly used in case analysis)

- **Minamata disease (Japan):** methylmercury (Hg) contaminated seafood; residents who ate it suffered central-nervous-system poisoning. → corresponds to "mercury monitoring." Ancient Romans using lead for cosmetic powder/water pipes is another example of lead harm.
- **Love Canal event:** a community built over buried hazardous chemical waste; residents fell ill and birth defects increased. → hazardous-waste landfill and leachate hazards.
- **Times Beach (USA):** dioxin contamination spread on roads; the whole town was evacuated. → incineration/dioxin, hazardous-waste standards.
- **Los Angeles photochemical smog:** vehicle-exhaust NOₓ + HC formed O₃ and PAN under ultraviolet light, irritating the eyes and harming plants. → secondary pollutants, photochemical smog.
- **Acid rain** (pH < 5.6): SO₂ → H₂SO₄, NOₓ → HNO₃. Southwest China is a heavy acid-rain region.

## 4.4 ⭐ Easily confused-concept distinctions (must-read before the exam)

| Confused pair | Key distinction |
|---|---|
| Composite vs. mixed water sample | Composite = simultaneous, different points; mixed = same point, different times |
| Class I vs. Class II pollutants (wastewater) | Class I sampled at the workshop outlet (highly toxic, source control); Class II sampled at the factory's main outlet |
| Acidity / alkalinity / pH | Acidity, alkalinity are neutralizing capacities (capacity concept); pH is H⁺ activity (intensity concept) |
| True color / apparent color | True color = color after removing suspended solids; apparent color = color without removing them |
| Total N / Kjeldahl N | Total N = organic N + ammonia-N + nitrite-N + nitrate-N; Kjeldahl N = organic N + ammonia-N (excludes nitrate/nitrite) |
| COD / permanganate index | Different oxidants: COD uses dichromate (oxidation rate ≈ 90%); permanganate index uses KMnO₄ (≈ 50%) |
| BOD / COD / TOC | BOD measures the biodegradable fraction; COD measures the fraction oxidizable by a strong oxidant; TOC measures all organic carbon by combustion. BOD/COD > 0.5 easy to treat biologically, < 0.3 contains toxics or needs acclimation |
| Primary / secondary pollutant | Primary = directly emitted, nature unchanged; secondary = new substances formed by reaction (O₃, PAN, etc.) |
| Molecular / particulate pollutant | Molecular state e.g. SO₂, CO; particulate state e.g. dustfall, TSP, PM |
| Dustfall / TSP / PM₁₀ / PM2.5 | > 100 μm dustfall; < 100 μm TSP; < 10 μm PM₁₀; < 2.5 μm PM2.5 |
| FID / ECD / TCD / FPD | FID universal for organics; ECD for electronegative substances (halogenated hydrocarbons, pesticides); TCD universal macro-quantity; FPD selective for S, P |
| Sound power / intensity / pressure | W (total energy, W); I (energy per unit area, W/m²); p (pressure increment, Pa); when adding, energy/intensity can be added, sound pressure cannot be added directly |
| α / β / γ decay | α emits ⁴He (heavy nuclei); β emits electrons (proton–neutron interconversion); γ emits electromagnetic radiation (energy-level transition) |
| Exposure / absorbed dose / dose equivalent | Exposure (air ionization, C/kg); absorbed dose (energy absorbed per unit mass, Gy); dose equivalent (considers biological effect, Sv) |
| Wet digestion / dry ashing | Wet uses acid oxidation; dry ashing ignites at 450–550 °C, cannot be used for volatile elements (As/Hg/Cd/Se/Sn) |
| Direct / enrichment sampling (gas) | Direct = high concentration, small gas sample; enrichment = low concentration (10⁻⁹–10⁻⁶), long duration, represents an average |

---

# Part 5　Quick-Memory Cards & Self-Test

## 5.1 Number quick-memory (high-frequency fill-in/multiple-choice)

- River reduction section: more than **1500 m** downstream of the last outlet.
- Vertical sampling: < 5 m one point; 5–10 m two points; > 10 m three points.
- Air layout: sector angle ≤ 90° (commonly 45°); grid downwind accounts for 60%; no source within 50 m, 270° space.
- Refrigerate 2–5 °C; freeze −20 °C; metals pH 1–2; cyanide/phenol pH 12; 0.45 μm membrane.
- BOD₅: 20 ± 1 °C, 5 days, dark; oxygen uptake > 2, residual > 2 (or 1) mg/L; dilution water pH 7.2, BOD₅ < 0.2; standard solution 180–230 mg/L.
- COD: > 50 use 0.25 mol/L, 5–50 use 0.025 mol/L dichromate.
- Hazardous waste: flash point < 60 °C; leachate pH ≤ 2 or ≥ 12.5; steel corrosion > 0.64 cm/a; natural radioactivity > 3700 Bq/kg.
- Soil: ≥ 3 points per unit; checkerboard solid-waste pollution > 20 points; composite sample farmland 0–20 cm, orchard 0–60 cm.
- Acoustic references: p₀ = 2 × 10⁻⁵ Pa; W₀ = I₀ = 10⁻¹² (W / W·m⁻²).
- Wavelengths: visible 400–780 nm; Hg 253.7 nm; SO₂ 577 nm; NOₓ 540 nm; FPD S 394 / P 526 nm.

## 5.2 Self-test points per chapter (if you can rattle them off, you've passed)

**Water:** ① The 6 objectives of water-quality monitoring? ② The four river cross-sections and the location of the reduction section? ③ Vertical layout by water depth? ④ The Class I/Class II distinction and sampling points? ⑤ The 4 categories of water-sample preservation with examples? ⑥ Common wet-digestion acid systems? Elements not suitable for dry ashing? ⑦ The DO iodometry reaction chain and the two corrections? ⑧ The COD formula, reagents, and interference handling? ⑨ BOD₅ conditions, dilution-water requirements, seeding, and nitrification? ⑩ The BOD/COD/TOC relationship and the meaning of the BOD/COD ratio? ⑪ The applicable targets of the four GC detectors?

**Air:** ① Primary/secondary pollutants, molecular/particulate state? ② Cause and products of photochemical smog? ③ Applicable situations of the three layout methods? ④ Direct vs. enrichment sampling? ⑤ Representative methods and wavelengths for SO₂, NOₓ, CO? ⑥ TSP/PM₁₀ determination (gravimetry, flow rate)? ⑦ How AQI and the primary pollutant are determined? ⑧ Stationary-source sampling location (downstream > 6D / upstream > 3D) and total pressure = static + dynamic? ⑨ Static/dynamic standard-gas preparation methods?

**Solid waste:** ① Identification of the 6 hazardous-waste characteristics? ② The leaching-toxicity test? ③ Basis for increment count/mass, the quartering method? ④ The three sampling depths for a transport truck? ⑤ High/low calorific value and the meaning of the conversion? ⑥ Why is leachate special?

**Soil:** ① The three-phase composition of soil and its proportions? ② Definition and role of the background value? ③ Applicability of the six layout methods? ④ Composite vs. profile sample, the A/B/C horizons? ⑤ The four digestion methods? ⑥ Single-factor/integrated pollution index and classification?

**Physical:** ① Sound power/intensity/pressure and the three level formulas? ② Why can't noise be added directly, and how is it calculated? ③ The meaning and calculation of Leq? ④ Characteristics of A-weighting? ⑤ α/β/γ decay? ⑥ Exposure/absorbed dose/dose equivalent?

---

> Suggested review route: first pass — read through to build the framework (focus on Parts 0 and 1) → second pass — study Parts 2 and 3 closely and work the example problems by hand → third pass — read only Parts 4 and 5 to fill gaps → finally, do the "mock exams" to test yourself. Good luck on the exam!

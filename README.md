# Field Trial Mixed Model Analysis (1968–2023)
**Modeling nitrogen response and cultivar performance across multi-season crop field trials**

This repository contains an end-to-end agronomy analytics pipeline using linear mixed-effects models to evaluate nitrogen fertilizer response and cultivar performance across 50+ years of field trial data.  

The analysis demonstrates real-world agricultural statistical workflows used in ag-biotech R&D and precision agriculture programs.

---

## 📌 Objectives

- Quantify yield response to nitrogen fertilizer across seasons
- Evaluate cultivar performance and stability across environments
- Correctly model a multi-year, multi-season **RCBD split-plot field design**
- Derive agronomic recommendations from statistical evidence
- Produce publication-quality visuals and interpretation

---

## 🧪 Experimental Design

| Component | Description |
|---|---|
Design | Split-plot RCBD |
Years | 1968–2023 |
Main plot | Nitrogen rate *(Afactor)* |
Sub plot | Cultivar *(Bfactor)* |
Blocks | 4 reps per year |
Seasons | DS, EWS, LWS |
Response | Grain yield (kg/ha) |

**Random Effects:** Year, Year × Rep × Nitrogen  
**Fixed Effects:** Season × Nitrogen + Season × Cultivar

---

## 🧰 Tech Stack

| Category | Tools |
|---|---|
Statistical Modeling | `lme4`, `lmerTest`, `emmeans` |
Data Manipulation | `dplyr`, `data.table` |
Visualization | `ggplot2`, `patchwork` |
Reporting | RMarkdown, GitHub |

---

## 📊 Key Results

### Nitrogen Response
- Dry season: strong yield increase up to **F4**
- Wet seasons: **yield plateau at F3** (no benefit from F4)

### Cultivar Performance
- **V4** highest and most stable across seasons  
- **V1** consistently lowest  
- Differences narrower in wet seasons due to environmental stress

---

## 🌾 Agronomic Recommendations

| Season | Optimal N | Insight |
|---|---|---|
Dry | **F4** | Highest N efficiency & yield gain |
Early Wet | **F3** | Output plateau; avoid excess N |
Late Wet | **F3** | Same plateau effect |

**Cultivar Recommendation:**  
Plant **V4** for broad seasonal adaptability; avoid **V1**.

---

## 📈 Visual Outputs

<p align="center">
<img src="plots/nitrogen_response.png" width="90%"><br>
<i>Nitrogen response across seasons (EMMs ± 95% CI)</i>
</p>

<p align="center">
<img src="plots/cultivar_response.png" width="90%"><br>
<i>Cultivar performance by season (EMMs ± 95% CI)</i>
</p>

---

## 📙 Methods

- Linear mixed-effects model
- Tukey adjusted marginal means
- Model hierarchy + interaction testing
- Confidence interval-based inference
- Agronomic interpretation & N-rate optimization

---

## 🔜 Future Extensions

- ✅ Spatial interpolation (kriging) for precision-ag layout
- ✅ Field-zone nitrogen recommendation maps
- ⏳ Random-slope G×E stability modeling (AMMI / GGE)
- ⏳ Power analysis for trial design efficiency

---

## 🚀 Why This Project Matters

This analysis mirrors real ag-biotech workflows used for:

- Biological product evaluation
- Nitrogen-use efficiency screening
- Cultivar stability assessments
- On-farm precision agriculture decision-support

It showcases expertise in:

- Experimental design interpretation
- Mixed-model statistical inference
- Field trial reporting & visualization
- Translating science → agronomy recommendations

---


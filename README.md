# The Impact of Economic Risk, Financial Risk, and Political Risk on Resource Sustainability  
### Method of Moments Quantile Regression and Club Convergence

<p align="center">
  <em></em><br>
  <em>Thesis Title</em><br>
  <em>Investigating the Impact of Foreign Direct Investment and Productive Capacity on Resource Sustainability</em><br>
</p>

<p align="center">

![Method1](https://img.shields.io/badge/Method1-Moment%20Quantile%20Regression-d1242f)
![Method2](https://img.shields.io/badge/Method2-Club%20Convergance-1f6feb)
![Period](https://img.shields.io/badge/Period-2000%E2%80%932021-2ea043)
![Countries](https://img.shields.io/badge/Countries-111-8250df)


</p>

---

## 📖 About the Thesis

This repository contains the research materials, empirical analysis, methodology, and thesis document for an **M.Sc. thesis in Economics** investigating the relationship between **Foreign Direct Investment**, **Productive Capacity**, **Economic Risk**, **Financial Risk**, **Political Risk**, and **Resource Sustainability**.

The empirical study examines **111 countries over the period 2000–2021** and focuses on whether economic activity and investment contribute to or undermine resource sustainability.

Rather than estimating only an average relationship across countries, the study combines two complementary approaches:

> **Club Convergence** identifies groups of countries that exhibit similar long-run patterns of resource sustainability, while **Method of Moments Quantile Regression (MMQR)** estimates heterogeneous effects across different levels of resource consumption.

The analysis incorporates:

- Foreign Direct Investment (**FDI**)
- Productive Capacity (**PCI**)
- Economic Risk (**ER**)
- Financial Risk (**FR**)
- Political Risk (**PR**)
- Gross Domestic Product per capita (**GDP**)
- Material Footprint per capita (**MFP**)

---

# 🎯 Research Question

The central research problem can be summarized as:

> **How do Foreign Direct Investment and Productive Capacity affect Resource Sustainability, and do these effects differ across countries with different levels of resource consumption and risk?**

The study addresses this by combining **cross-country heterogeneity**, **convergence behavior**, and **distributional econometric analysis**.

---

## 🎓 Thesis Information

| | |
| **Author** | Amin Mirhaj |
| **Degree** | M.Sc. in Economics |
| **University** | Ferdowsi University of Mashhad |
| **Supervisor** | Dr. Narges Salehnia |
| **Advisor** | Dr. Fariba Osmani |
| **Published Year** | 2024 |

### 📄 Full Thesis

**[View Full Thesis →](./thesis/thesis.pdf)**

---

# 🗂️ Repository Structure

```text
master-thesis-quantitative-econometrics/
│
├── 📄 README.md
│
├── 📚 thesis/
│   └── thesis.pdf
│
├── 📊 data/
│   ├── raw/
│   ├── processed/
│   └── README.md
│
├── 💻 code/
│   ├── python/
│   └── stata/
│
├── 📓 notebooks/
│   ├── 01_data_preparation.ipynb
│   ├── 02_eda.ipynb
│   ├── 03_club_convergence.ipynb
│   ├── 04_panel_diagnostics.ipynb
│   ├── 05_mmqr.ipynb
│   └── 06_results_visualization.ipynb
│
├── 📈 results/
│   ├── tables/
│   └── figures/
│
└── 📑 docs/
    ├── data_sources.md
    ├── methodology.md
    └── variable_dictionary.md
```

---

# 🧭 Research at a Glance

```mermaid
flowchart LR
    A["🌍 111 Countries<br/>2000–2021"]
    B["📦 Resource Sustainability<br/>Material Footprint per Capita"]
    C["💰 Foreign Direct Investment<br/>FDI"]
    D["🏭 Productive Capacity<br/>PCI"]
    E["⚠️ Country Risk"]
    F["📈 GDP per Capita"]

    E --> E1["Economic Risk"]
    E --> E2["Financial Risk"]
    E --> E3["Political Risk"]

    A --> B
    C --> B
    D --> B
    E1 --> B
    E2 --> B
    E3 --> B
    F --> B

    B --> G["🔬 Empirical Analysis"]

    G --> H["Club Convergence"]
    G --> I["MMQR"]

    H --> J["Identify Convergence Clubs"]
    J --> I

    I --> K["Quantile-Specific Effects"]
    K --> L["📊 Results & Policy Implications"]
```

---

# 🔬 Research Methodology

The empirical workflow follows a sequential design:

```mermaid
flowchart TD

    A["01 · Data Collection"] --> B["02 · Data Cleaning & Integration"]
    B --> C["03 · Variable Construction"]
    C --> D["04 · Exploratory Analysis"]
    D --> E["05 · Panel Diagnostics"]

    E --> E1["Cross-Sectional Dependence"]
    E --> E2["Slope Heterogeneity"]
    E --> E3["Panel Unit Root"]
    E --> E4["Panel Cointegration"]

    E1 --> F["06 · Club Convergence"]
    E2 --> F
    E3 --> F
    E4 --> F

    F --> G["Identify Convergence Clubs"]

    G --> H["07 · MMQR Estimation"]

    H --> H1["Q10"]
    H --> H2["Q25"]
    H --> H3["Q50"]
    H --> H4["Q75"]
    H --> H5["Q90"]

    H1 --> I["Distributional Effects"]
    H2 --> I
    H3 --> I
    H4 --> I
    H5 --> I

    I --> J["08 · Robustness Analysis"]
    J --> K["09 · Results & Visualization"]
    K --> L["10 · Economic & Policy Interpretation"]
```

---

# 🌍 Method 1 — Club Convergence

A key feature of the research is the use of **Club Convergence**.

Instead of assuming that all 111 countries follow the same long-run trajectory, countries are grouped according to their convergence behavior in resource sustainability.

```mermaid
flowchart TD

    A["🌍 111 Countries"] --> B["Club Convergence Analysis"]

    B --> C["Convergence Structure"]

    C --> D["🔵 Club 1<br/>67 Countries"]
    C --> E["🟣 Club 2<br/>44 Countries"]

    D --> F["Club-Specific Analysis"]
    E --> F

    F --> G["MMQR Estimation"]
```

### Identified structure

| Convergence Club | Number of Countries |
|---|---:|
| **Club 1** | 67 |
| **Club 2** | 44 |
| **Total** | **111** |

The resulting clubs are then analyzed separately in order to capture differences in the underlying country groups.

---

# 📐 Method 2 — Method of Moments Quantile Regression

The main econometric technique is **Method of Moments Quantile Regression (MMQR)**.

Unlike conventional mean regression, MMQR allows the analysis to examine relationships at different points of the conditional distribution of Material Footprint per capita.

```mermaid
flowchart TB

    A["Conditional Distribution<br/>of Material Footprint per Capita"]

    A --> Q10["Q10<br/>Lower MFP"]
    A --> Q25["Q25"]
    A --> Q50["Q50<br/>Median"]
    A --> Q75["Q75"]
    A --> Q90["Q90<br/>Higher MFP"]

    Q10 --> M["MMQR"]
    Q25 --> M
    Q50 --> M
    Q75 --> M
    Q90 --> M

    M --> R["Heterogeneous<br/>Distributional Effects"]
```

### Quantiles examined

**Q10 · Q25 · Q50 · Q75 · Q90**

This allows the research to ask a more detailed question:

> Do FDI, productive capacity, risk, and GDP have the same relationship with resource consumption across the distribution?

---

# 📈 What Makes the Empirical Strategy Different?

The research combines **three dimensions of heterogeneity**:

```mermaid
flowchart LR

    A["Country Heterogeneity"]
    B["Long-Run Convergence"]
    C["Distributional Heterogeneity"]

    A --> D["More Detailed<br/>Empirical Analysis"]
    B --> D
    C --> D

    D --> E["Resource Sustainability"]
```

### 1. Country heterogeneity

Countries are not assumed to behave identically.

### 2. Convergence heterogeneity

Countries are grouped into convergence clubs based on their long-run resource-sustainability patterns.

### 3. Distributional heterogeneity

MMQR evaluates effects at different quantiles rather than only estimating an average effect.

Together, these approaches provide a more granular empirical framework for studying resource sustainability.

---

# 🔬 Reproducibility Workflow

The intended workflow for reproducing the empirical analysis is:

```mermaid
sequenceDiagram

    participant D as Data
    participant P as Preparation
    participant E as Econometrics
    participant R as Results
    participant T as Thesis

    D->>P: Raw datasets
    P->>P: Clean & integrate
    P->>E: Panel dataset
    E->>E: Diagnostics
    E->>E: Club convergence
    E->>E: MMQR estimation
    E->>R: Estimates
    R->>R: Tables & figures
    R->>T: Empirical results
```

---

# 🗃️ Data Sources

The thesis integrates information from several major databases:

| Source | Main Contribution |
|---|---|
| **Global Material Flows Database (GMFD)** | Material Footprint |
| **UNCTAD** | Foreign Direct Investment / Productive Capacity |
| **International Country Risk Guide (ICRG)** | Country Risk |
| **World Development Indicators (WDI)** | GDP and macroeconomic indicators |

---

# 📝 Methodological Summary

| Stage | Method / Component | Purpose |
|---|---|---|
| **1** | Data collection | Construct the country-level panel |
| **2** | Data cleaning & integration | Prepare consistent empirical data |
| **3** | Variable construction | Define MFP, FDI, PCI, risk variables and GDP |
| **4** | Exploratory analysis | Understand the data |
| **5** | Panel diagnostics | Assess dependence, heterogeneity, stationarity and long-run relationships |
| **6** | Club Convergence | Identify groups with similar long-run patterns |
| **7** | MMQR | Estimate heterogeneous distributional effects |
| **8** | Robustness analysis | Assess the stability of findings |
| **9** | Visualization | Present empirical evidence |
| **10** | Interpretation | Derive economic and policy implications |

---

# 🔑 Keywords

`Resource Sustainability` · `Foreign Direct Investment` · `Productive Capacity` · `Economic Risk` · `Financial Risk` · `Political Risk` · `Panel Data` · `Club Convergence` · `Method of Moments Quantile Regression`

---

# 📄 Citation

For users of this repository or thesis, the recommended reference is:

```text
Suggested citation:
Mirhaj, A. (2024). Investigating the Impact of Foreign Direct Investment and Productive Capacity on Resource Sustainability: Method of Moments Quantile Regression and Club Convergence (M.Sc. thesis). Ferdowsi University of Mashhad.
```

---

<p align="center">
  <strong>https://github.com/aminmirhaj/master-thesis-quantitative-econometrics</strong>
</p>

<p align="center">
  <a href="./thesis/thesis.pdf">📄 Read the Full Thesis</a>
</p>
# The Impact of Economic Risk, Financial Risk, and Political Risk on Resource Sustainability  
### Method of Moments Quantile Regression and Club Convergence

<p align="center">
  <em></em><br>
  <em>Thesis Title</em><br>
  <em>Investigating the Impact of Foreign Direct Investment and Productive Capacity on Resource Sustainability</em><br>
</p>

<p align="center">

![Econometric](https://img.shields.io/badge/Econometric-Method%20of%20Moment%20Quantile%20Regression-d1242f)
![Econometric](https://img.shields.io/badge/Econometric-Club%20Convergance-1f6feb)
![Period](https://img.shields.io/badge/Period-2000%E2%80%932021-2ea043)
![Countries](https://img.shields.io/badge/Countries-111-8250df)


</p>

---

## 📖 About the Thesis

This repository contains the research materials, empirical analysis, methodology, and thesis document for an **M.Sc. thesis in Economics** investigating the relationship between **Foreign Direct Investment (FDI)**, **Productive Capacity**, country-level risks, and **Resource Sustainability**.

The empirical study examines **111 countries over the period 2000–2021** and focuses on whether economic activity and investment contribute to or undermine resource sustainability.

Rather than estimating only an average relationship across countries, the study combines two complementary approaches:

> **Club Convergence** identifies groups of countries that exhibit similar long-run patterns of resource sustainability, while **Method of Moments Quantile Regression (MMQR)** estimates heterogeneous effects across different levels of resource consumption.

The analysis incorporates:

- Foreign Direct Investment (**FDI**)
- Productive Capacity (**PCI**)
- Economic Risk (**ER**)
- Financial Risk (**FR**)
- Political Risk (**PR**)
- GDP per capita
- Material Footprint per capita (**MFP**)

---

## 🎓 Thesis Information

| | |
|---|---|
| **Author** | Amin Mirhaj |
| **Degree** | M.Sc. in Economics |
| **University** | Ferdowsi University of Mashhad |
| **Supervisor** | Dr. Narges Salehnia |
| **Advisor** | Dr. Fariba Osmani |
| **Year** | 2024 |
| **Countries** | 111 |
| **Study Period** | 2000–2021 |

### 📄 Full Thesis

**[View Full Thesis →](./thesis/thesis.pdf)**

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

# 🎯 Research Question

The central research problem can be summarized as:

> **How do Foreign Direct Investment and Productive Capacity affect Resource Sustainability, and do these effects differ across countries with different levels of resource consumption and risk?**

The study addresses this by combining **cross-country heterogeneity**, **convergence behavior**, and **distributional econometric analysis**.

---

# 🧩 Conceptual Framework

The conceptual structure of the study is centered on **Material Footprint per capita (MFP)** as the indicator of resource consumption/sustainability.

```mermaid
flowchart TB

    subgraph ECONOMIC["Economic & Investment Factors"]
        FDI["Foreign Direct Investment<br/>(FDI)"]
        PCI["Productive Capacity<br/>(PCI)"]
        GDP["GDP per Capita"]
    end

    subgraph RISK["Country Risk"]
        ER["Economic Risk<br/>(ER)"]
        FR["Financial Risk<br/>(FR)"]
        PR["Political Risk<br/>(PR)"]
    end

    FDI --> MFP["Material Footprint per Capita<br/>(MFP)"]
    PCI --> MFP
    GDP --> MFP
    ER --> MFP
    FR --> MFP
    PR --> MFP

    MFP --> S["Resource Sustainability"]

    style MFP stroke-width:3px
    style S stroke-width:3px
```

### Core interpretation

The framework does not assume that the relationships are identical for all countries. Instead, the empirical strategy explicitly investigates **heterogeneous effects across the conditional distribution of MFP**.

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

# 🧪 Step 1 — Data Preparation

The study combines country-level information into a panel dataset covering:

> **111 countries × 2000–2021**

The principal variables are:

| Variable | Role | Description |
|---|---|---|
| **MFP** | Dependent variable | Material Footprint per capita |
| **FDI** | Explanatory variable | Foreign Direct Investment |
| **PCI** | Explanatory variable | Productive Capacity |
| **ER** | Risk variable | Economic Risk |
| **FR** | Risk variable | Financial Risk |
| **PR** | Risk variable | Political Risk |
| **GDP** | Control variable | GDP per capita |

---

# 📊 Step 2 — Panel Data Diagnostics

Before estimating the main models, the panel structure is examined through a series of diagnostic procedures.

```mermaid
flowchart LR

    DATA["Panel Dataset"]

    DATA --> CD["Cross-Sectional<br/>Dependence"]
    DATA --> SH["Slope<br/>Heterogeneity"]
    DATA --> UR["Panel<br/>Unit Root"]
    DATA --> CO["Panel<br/>Cointegration"]

    CD --> VALID["Econometric<br/>Model Validation"]
    SH --> VALID
    UR --> VALID
    CO --> VALID

    VALID --> EST["MMQR Estimation"]
```

### Diagnostic objectives

- **Cross-sectional dependence** → assess whether countries are interdependent.
- **Slope heterogeneity** → assess whether relationships differ across countries.
- **Panel unit root** → evaluate the time-series properties of the variables.
- **Panel cointegration** → investigate long-run relationships.

These diagnostics provide the foundation for the subsequent empirical estimation.

---

# 🌍 Step 3 — Club Convergence

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

# 📐 Step 4 — Method of Moments Quantile Regression

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

# 🔗 Integrated Empirical Strategy

The complete research design can be represented as:

```mermaid
flowchart TD

    A["🌍 111 Countries<br/>2000–2021"]

    A --> B["📦 Panel Dataset"]

    B --> C["Panel Diagnostics"]

    C --> D["Club Convergence"]

    D --> E1["Club 1<br/>67 Countries"]
    D --> E2["Club 2<br/>44 Countries"]

    E1 --> F["MMQR"]
    E2 --> F

    subgraph X["Explanatory Variables"]
        X1["FDI"]
        X2["PCI"]
        X3["Economic Risk"]
        X4["Financial Risk"]
        X5["Political Risk"]
        X6["GDP per Capita"]
    end

    X1 --> F
    X2 --> F
    X3 --> F
    X4 --> F
    X5 --> F
    X6 --> F

    F --> Q["Q10 · Q25 · Q50 · Q75 · Q90"]

    Q --> R["Distributional Effects"]

    R --> S["Robustness Analysis"]

    S --> T["📊 Results"]

    T --> U["💡 Economic & Policy Implications"]
```

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

# 🗃️ Data Sources

The thesis integrates information from several major databases:

| Source | Main Contribution |
|---|---|
| **Global Material Flows Database (GMFD)** | Material Footprint |
| **UNCTAD** | Foreign Direct Investment / Productive Capacity |
| **International Country Risk Guide (ICRG)** | Country Risk |
| **World Development Indicators (WDI)** | GDP and macroeconomic indicators |

---

# 🧮 Variable Map

```mermaid
flowchart TB

    M["Material Footprint<br/>per Capita"]

    FDI["FDI"]
    PCI["Productive Capacity"]
    ER["Economic Risk"]
    FR["Financial Risk"]
    PR["Political Risk"]
    GDP["GDP per Capita"]

    FDI --> M
    PCI --> M
    ER --> M
    FR --> M
    PR --> M
    GDP --> M

    M --> Y["Resource Sustainability<br/>Outcome"]
```

---

# 📚 Research Pipeline

For reproducibility, the repository follows a logical progression from raw data to final empirical results:

```mermaid
flowchart LR

    A["Raw Data"] --> B["Processed Data"]
    B --> C["Exploratory Analysis"]
    C --> D["Diagnostics"]
    D --> E["Club Convergence"]
    E --> F["MMQR"]
    F --> G["Robustness"]
    G --> H["Tables & Figures"]
    H --> I["Thesis Results"]
```

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

# 📊 Results Organization

The empirical results are organized around the main stages of the methodology:

```text
Results
│
├── 01 · Descriptive / Exploratory Analysis
│
├── 02 · Panel Diagnostics
│
├── 03 · Club Convergence
│     ├── Club 1
│     └── Club 2
│
├── 04 · MMQR Estimates
│     ├── Q10
│     ├── Q25
│     ├── Q50
│     ├── Q75
│     └── Q90
│
├── 05 · Robustness Analysis
│
└── 06 · Visualization
```

---

# 🧠 Research Logic in One Diagram

```mermaid
flowchart TB

    START(["Research Problem"])

    START --> QUESTION["How do investment,<br/>productive capacity and risk<br/>relate to resource sustainability?"]

    QUESTION --> DATA["111 Countries<br/>2000–2021"]

    DATA --> DIAG["Panel Diagnostics"]

    DIAG --> CLUB["Club Convergence"]

    CLUB --> CLUB1["Club 1<br/>67 Countries"]
    CLUB --> CLUB2["Club 2<br/>44 Countries"]

    CLUB1 --> MMQR["MMQR"]
    CLUB2 --> MMQR

    MMQR --> DIST["Q10 · Q25 · Q50 · Q75 · Q90"]

    DIST --> HET["Heterogeneous Effects"]

    HET --> ROB["Robustness Analysis"]

    ROB --> POLICY["Economic & Policy<br/>Implications"]

    POLICY --> END(["Resource Sustainability"])
```

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

# 🌱 Research Contribution

The empirical design provides a framework for examining resource sustainability that goes beyond a single average coefficient.

The combination of:

**Panel Data**  
↓  
**Club Convergence**  
↓  
**Club-Specific Analysis**  
↓  
**MMQR**  
↓  
**Quantile-Specific Effects**

allows the research to investigate whether the relationships between investment, productive capacity, country risk, GDP, and resource consumption vary across different groups and levels of resource use.

---

# 🔑 Keywords

`Resource Sustainability` · `Material Footprint` · `Foreign Direct Investment` · `Productive Capacity` · `Economic Risk` · `Financial Risk` · `Political Risk` · `Panel Data` · `Club Convergence` · `MMQR` · `Method of Moments Quantile Regression` · `Quantitative Economics` · `Econometrics`

---

# 📄 Citation

If you use this repository or thesis in your research, please cite:

```text
Mirhaj, Amin (2024).
The Impact of Economic Risk, Financial Risk, and Political Risk on Resource Sustainability:
Method of Moments Quantile Regression and Club Convergence.
M.Sc. Thesis, Ferdowsi University of Mashhad.
```

---

<p align="center">
  <strong>A quantitative investigation of investment, risk, and resource sustainability.</strong>
</p>

<p align="center">
  <a href="./thesis/thesis.pdf">📄 Read the Full Thesis</a>
</p>
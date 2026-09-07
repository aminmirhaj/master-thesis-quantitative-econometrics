# The Impact of Economic Risk, Financial Risk, and Political Risk on Resource Sustainability: Method of Moments Quantile Regression and Club Convergence

**Full Title:**  
*Investigating the Impact of Foreign Direct Investment and Productive Capacity on Resource Sustainability: Method of Moments Quantile Regression and Club Convergence*

**Author:**  
Amin Mirhaj

**Degree:**  
M.Sc. in Economics

**University:**  
Ferdowsi University of Mashhad

**Supervisor:**  
Dr. Narges Salehnia

**Advisor:**  
Dr. Fariba Osmani

**Year:**  
2024


[📄 View Full Thesis](./thesis/thesis.pdf)


---


## 🎯 Research Overview

This thesis examines whether **Foreign Direct Investment and Productive Capacity** contribute to or undermine **Resource Sustainability**, across **111** countries during **2000–2021**. The core problem is how to support economic development and investment while limiting increasing pressure on natural resources.

The empirical analysis first uses **Club Convergence** to identify groups of countries with similar long-run patterns of resource sustainability. It then applies **Method of Moments Quantile Regression (MMQR)** within the identified clubs to estimate how variables affect different levels of resource consumption, while accounting for **Economic, Financial, and Political Risks and GDP**.

The study therefore focuses on **heterogeneous country-level effects**, rather than relying only on average relationships. Its results aim to provide quantitative evidence for designing investment and development policies that can reconcile **economic growth with sustainable resource use**.


---

## 🧩 Research Architecture

```text
                    COUNTRY-LEVEL DATA
                           │
          ┌────────────────┼────────────────┐
          │                │                │
          ▼                ▼                ▼
        FDI               PCI          COUNTRY RISK
                                     
                                  ┌──────────────┐
                                  │Economic Risk │
                                  │Financial Risk│
                                  │Political Risk│
                                  └──────────────┘
          │                │                │
          └────────────────┼────────────────┘
                           │
                           ▼
                     PANEL DATASET
                     111 Countries
                       2000–2021
                           │
                           ▼
                   MATERIAL FOOTPRINT
                       PER CAPITA
                         (MFP)
```

---

## 🔬 Methodological Framework

```text
                    DATA COLLECTION
                           │
                           ▼
                  DATA CLEANING &
                     INTEGRATION
                           │
                           ▼
                 VARIABLE CONSTRUCTION
                           │
          ┌────────────────┼────────────────┐
          │                │                │
          ▼                ▼                ▼
         FDI               PCI          RISK VARIABLES
                                           │
                                  ┌────────┼────────┐
                                  ▼        ▼        ▼
                                 ER       FR       PR
                           Economic    Financial   Political
                               Risk         Risk        Risk
                           │
                           ▼
                  EXPLORATORY ANALYSIS
                           │
                           ▼
                 PANEL DATA DIAGNOSTICS
                           │
          ┌────────────────┼────────────────────┐
          ▼                ▼                    ▼
   Cross-sectional    Slope Heterogeneity   Unit Root
     Dependence
          │                │                    │
          └────────────────┼────────────────────┘
                           │
                           ▼
                     Cointegration
                           │
                           ▼
                   CLUB CONVERGENCE
                           │
                 ┌─────────┴─────────┐
                 ▼                   ▼
              CLUB 1              CLUB 2
            67 Countries         44 Countries
                 │                   │
                 └─────────┬─────────┘
                           ▼
                 MMQR ESTIMATION
                           │
                           ▼
              DISTRIBUTIONAL EFFECTS
                           │
                           ▼
                  ROBUSTNESS ANALYSIS
                           │
                           ▼
                 RESULTS & VISUALIZATION
```

---

## 📊 Econometric Structure

```text
                    MATERIAL FOOTPRINT
                       PER CAPITA
                           │
                           ▲
                           │
        ┌──────────────────┼──────────────────┐
        │                  │                  │
        │                  │                  │
       FDI                 PCI             RISK
                                           │
                              ┌────────────┼────────────┐
                              │            │            │
                         Economic      Financial     Political
                            Risk          Risk          Risk
        │                  │                  │
        └──────────────────┼──────────────────┘
                           │
                      GDP per Capita
                           │
                           ▼
                    MMQR ESTIMATION
                           │
                           ▼
                 Quantile-specific
                      Effects
```

---

## 📈 Club Convergence

Countries are first analyzed using **Club Convergence** to identify groups with similar long-run patterns in resource consumption.

```text
                  111 COUNTRIES
                        │
                        ▼
                CLUB CONVERGENCE
                        │
              ┌─────────┴─────────┐
              ▼                   ▼
           CLUB 1              CLUB 2
        67 Countries         44 Countries
              │                   │
              └─────────┬─────────┘
                        ▼
                  Separate Analysis
                        │
                        ▼
                       MMQR
```

---

## 📐 MMQR Framework

The main estimation method is **Method of Moments Quantile Regression (MMQR)**.

```text
                 CONDITIONAL DISTRIBUTION
                         OF MFP
                           │
       ┌─────────┬─────────┼─────────┬─────────┐
       ▼         ▼         ▼         ▼         ▼
     Q10       Q25       Q50       Q75       Q90
       │         │         │         │         │
       └─────────┴─────────┼─────────┴─────────┘
                           ▼
                         MMQR
                           │
                           ▼
                 HETEROGENEOUS EFFECTS
```

This allows the analysis to investigate whether the relationships differ across countries with different levels of resource consumption.

---

## 🧪 Panel Diagnostics

```text
Panel Dataset
     │
     ├── Normality
     │
     ├── Cross-sectional Dependence
     │
     ├── Slope Heterogeneity
     │
     ├── Panel Unit Root
     │
     ├── Panel Cointegration
     │
     └── Model Specification
             │
             ▼
       Econometric Estimation
```

---

## 📁 Repository Structure

```text
master-thesis-quantitative-econometrics/
│
├── README.md
│
├── thesis/
│   └── thesis.pdf
│
├── data/
│   ├── raw/
│   ├── processed/
│   └── README.md
│
├── code/
│   ├── python/
│   └── stata/
│
├── notebooks/
│   ├── 01_data_preparation.ipynb
│   ├── 02_eda.ipynb
│   ├── 03_club_convergence.ipynb
│   ├── 04_panel_diagnostics.ipynb
│   ├── 05_mmqr.ipynb
│   └── 06_results_visualization.ipynb
│
├── results/
│   ├── tables/
│   └── figures/
│
└── docs/
    ├── data_sources.md
    ├── methodology.md
    └── variable_dictionary.md
```

---

## 📚 Data Sources

The thesis integrates data from:

- **Global Material Flows Database (GMFD)** — Material Footprint
- **UNCTAD** — Foreign Direct Investment / Productive Capacity
- **International Country Risk Guide (ICRG)** — Country Risk
- **World Development Indicators (WDI)** — GDP and macroeconomic indicators

---

## 🔑 Keywords

`Quantitative Analysis` `Econometrics` `Panel Data` `Method of Moments Quantile Regression` `Club Convergence` `Economic Risk` `Financial Risk` `Political Risk` `Foreign Direct Investment` `Productive Capacity` `Resource Sustainability`
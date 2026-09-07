# The Impact of Economic, Financial, and Political Risk on Resource Sustainability

### Investigating the Impact of Foreign Direct Investment and Productive Capacity on Resource Sustainability Using MMQR and Club Convergence

<p align="center">

**M.Sc. Thesis in Economics**

**Ferdowsi University of Mashhad · 2024**

**Author:** Amin Mirhaj  
**Supervisor:** Dr. Narges Salehnia  
**Advisor:** Dr. Fariba Osmani

</p>

---

## 📄 Thesis

This repository contains the complete PDF version of my master's thesis.

The research investigates the relationship between **Resource Sustainability**, **Foreign Direct Investment (FDI)**, **Productive Capacity**, and **Economic, Financial, and Political Risk**.

The empirical analysis combines two main econometric approaches:

- **Club Convergence** — to identify groups of countries following similar long-run patterns of resource sustainability.
- **Method of Moments Quantile Regression (MMQR)** — to examine heterogeneous effects across different levels of resource consumption.

The study covers **111 countries over the period 2000–2021**.

### Read the Full Thesis

> 📖 **[Open the Complete Thesis →](./thesis.pdf)**

---

# 📚 Table of Contents

| Chapter | Title | Page |
|:---:|---|:---:|
| **01** | [Research Overview](#01--research-overview) | 2 |
| **02** | [Literature Review](#02--literature-review) | 14 |
| **03** | [Research Methodology](#03--research-methodology) | 37 |
| **04** | [Analysis of Findings](#04--analysis-of-findings) | 51 |
| **05** | [Conclusions & Recommendations](#05--conclusions--recommendations) | 76 |
| — | [References](#references) | 84 |
| — | [Appendix](#appendix) | 91 |

---

# 01 — Research Overview

> **Purpose:** Establishes the research problem, motivation, objectives, questions, methodology, and applications.

### 1.1 Introduction

### 1.2 Problem Statement

### 1.3 Research Necessity and Significance

### 1.4 Research Objectives

### 1.5 Research Questions

### 1.6 Research Methodology

- **1.6.1** Study Population
- **1.6.2** Sampling Method
- **1.6.3** Data Collection Method and Instruments
- **1.6.4** Data Analysis Method

### 1.7 Applications of the Research

[↑ Back to Table of Contents](#-table-of-contents)

---

# 02 — Literature Review

> **Purpose:** Develops the theoretical foundation and reviews previous international and domestic research.

## 2.1 Introduction

## 2.2 Theoretical Foundations

### 2.2.1 Resource Sustainability

### 2.2.2 Foreign Direct Investment

### 2.2.3 Productive Capacity

### 2.2.4 Economic, Financial, and Political Risk

- **2.2.4.1** Economic Risk
- **2.2.4.2** Financial Risk
- **2.2.4.3** Political Risk

### 2.2.5 Gross Domestic Product

## 2.3 Research Background

- **2.3.1** International Studies
- **2.3.2** Domestic Studies

## 2.4 Summary and Conclusions

[↑ Back to Table of Contents](#-table-of-contents)

---

# 03 — Research Methodology

> **Purpose:** Presents the research model, variables, data sources, preliminary tests, and econometric methods.

## 3.1 Introduction

## 3.2 Research Model

### 3.2.1 Definitions and Sources of Variables

- **3.2.1.1** Dependent Variable
- **3.2.1.2** Main Independent Variables
- **3.2.1.3** Control Variables

## 3.3 Research Methodology

### Preliminary Tests

| Test | Purpose |
|---|---|
| **3.3.1.1 Limer Test** | Model specification |
| **3.3.1.2 Non-Normality Test** | Distributional properties |
| **3.3.1.3 Cross-Sectional Dependence Test** | Dependence across countries |
| **3.3.1.4 Slope Heterogeneity Test** | Heterogeneous coefficients |
| **3.3.1.5 Unit Root Test** | Panel stationarity |
| **3.3.1.6 Cointegration Test** | Long-run relationships |

### Econometric Approaches

#### 3.3.2 — Club Convergence

Identifies groups of countries exhibiting similar long-run dynamics in resource sustainability.

#### 3.3.3 — Method of Moments Quantile Regression

Examines how the explanatory variables affect different points of the conditional distribution rather than only estimating an average effect.

## 3.4 Summary and Conclusions

[↑ Back to Table of Contents](#-table-of-contents)

---

# 04 — Analysis of Findings

> **Purpose:** Presents the empirical results, convergence analysis, descriptive statistics, model estimation, and robustness analysis.

## 4.1 Introduction

## 4.2 Results of the Club Convergence Approach

- **4.2.1** Test Results
- **4.2.2** Clustering Club Test Results
- **4.2.3** Club Merging Results

## 4.3 Trends of the Main Research Variables

- **4.3.1** Resource Sustainability Trends
- **4.3.2** Foreign Direct Investment Trends

## 4.4 Descriptive Statistics

## 4.5 Model Specification

## 4.6 Model Estimation Results

### 4.6.1 Preliminary Test Results

- **4.6.1.1** Limer Test Results
- **4.6.1.2** Non-Normality Test Results
- **4.6.1.3** Cross-Sectional Dependence Test Results
- **4.6.1.4** Slope Heterogeneity Test Results
- **4.6.1.5** Unit Root Test Results
- **4.6.1.6** Cointegration Test Results

### 4.6.2 Moment Quantile Regression Results

### 4.6.3 Final Test Results

- **4.6.3.1** Robustness Test Results

## 4.7 Summary and Conclusions

[↑ Back to Table of Contents](#-table-of-contents)

---

# 05 — Conclusions & Recommendations

> **Purpose:** Summarizes the empirical findings and translates the results into conclusions and recommendations.

## 5.1 Introduction

## 5.2 Conclusions

## 5.3 Answers to the Research Questions

## 5.4 Recommendations

### 5.4.1 Policy Recommendations

### 5.4.2 Recommendations for Future Research

[↑ Back to Table of Contents](#-table-of-contents)

---

# 🔬 Research Framework

The thesis follows a two-stage empirical framework.

```text
                         111 COUNTRIES
                          2000–2021
                               │
                               ▼
                    ┌─────────────────────┐
                    │     PANEL DATA      │
                    └──────────┬──────────┘
                               │
             ┌─────────────────┼─────────────────┐
             │                 │                 │
             ▼                 ▼                 ▼
            FDI                PCI              RISK
                                                │
                                     ┌──────────┼──────────┐
                                     ▼          ▼          ▼
                                    ER         FR         PR
                               Economic    Financial   Political
                                  Risk        Risk        Risk
             │                 │                 │
             └─────────────────┼─────────────────┘
                               │
                               ▼
                  ┌─────────────────────────┐
                  │   RESOURCE SUSTAINABILITY│
                  │      / MATERIAL FOOTPRINT│
                  └────────────┬────────────┘
                               │
                               ▼
                     ┌──────────────────┐
                     │ CLUB CONVERGENCE │
                     └────────┬─────────┘
                              │
                    ┌─────────┴─────────┐
                    ▼                   ▼
                 CLUB 1              CLUB 2
              67 Countries         44 Countries
                    │                   │
                    └─────────┬─────────┘
                              │
                              ▼
                    ┌──────────────────┐
                    │       MMQR       │
                    └────────┬─────────┘
                             │
             ┌───────────────┼───────────────┐
             ▼               ▼               ▼
           Q10             Q50             Q90
             │               │               │
             └───────────────┼───────────────┘
                             ▼
                  HETEROGENEOUS EFFECTS
                             │
                             ▼
                    ROBUSTNESS ANALYSIS
                             │
                             ▼
                       FINAL RESULTS
```

---

# 📐 Econometric Approaches

## Club Convergence

The first stage identifies groups of countries that exhibit similar long-run patterns of resource sustainability.

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

## Method of Moments Quantile Regression

The second stage applies **MMQR** to investigate whether the effects of the explanatory variables vary across different levels of resource consumption.

```text
                 CONDITIONAL DISTRIBUTION
                         OF MFP
                           │
          ┌────────┬───────┼───────┬────────┐
          ▼        ▼       ▼       ▼        ▼
         Q10      Q25     Q50     Q75      Q90
          │        │       │       │        │
          └────────┴───────┼───────┴────────┘
                           ▼
                          MMQR
                           │
                           ▼
                  HETEROGENEOUS EFFECTS
```

This approach allows the analysis to move beyond an average-effect interpretation and examine how relationships differ across the conditional distribution.

---

# 🧪 Panel Data Diagnostics

Before the final estimation, the empirical framework incorporates a sequence of panel-data diagnostic tests.

```text
                     PANEL DATASET
                           │
                           ▼
                  MODEL SPECIFICATION
                           │
                           ▼
        ┌──────────────────┼──────────────────┐
        │                  │                  │
        ▼                  ▼                  ▼
    Normality      Cross-Sectional     Slope Heterogeneity
                       Dependence
        │                  │                  │
        └──────────────────┼──────────────────┘
                           ▼
                     Unit Root Test
                           │
                           ▼
                    Cointegration
                           │
                           ▼
                   Club Convergence
                           │
                           ▼
                         MMQR
                           │
                           ▼
                  Robustness Analysis
```

---

# 📊 Key Research Variables

| Category | Variable |
|---|---|
| **Dependent Variable** | Resource Sustainability / Material Footprint per Capita (MFP) |
| **Main Independent Variable** | Foreign Direct Investment (FDI) |
| **Main Independent Variable** | Productive Capacity (PCI) |
| **Risk Variables** | Economic Risk (ER) |
| **Risk Variables** | Financial Risk (FR) |
| **Risk Variables** | Political Risk (PR) |
| **Control Variable** | GDP |

---

# 🌍 Study Coverage

| Dimension | Coverage |
|---|---|
| **Countries** | 111 |
| **Period** | 2000–2021 |
| **Unit of Analysis** | Country |
| **Data Structure** | Panel Data |
| **Convergence Analysis** | Club Convergence |
| **Main Estimation** | MMQR |
| **Main Outcome** | Material Footprint per Capita |

---

# 📚 References

The thesis concludes with the complete list of academic sources and references used throughout the research.

[↑ Back to Table of Contents](#-table-of-contents)

---

# 📎 Appendix

Additional tables, materials, and supporting information are provided in the appendix.

[↑ Back to Table of Contents](#-table-of-contents)

---

# 📁 Repository Structure

Because the README is located **in the same directory as the thesis PDF**, the repository can remain simple:

```text
.
├── README.md
└── thesis.pdf
```

---

## 📖 Full Thesis

The complete thesis is available as a PDF:

**[📄 Read the Full Thesis →](./thesis.pdf)**

---

<p align="center">

**M.Sc. Economics · Ferdowsi University of Mashhad · 2024**

</p>
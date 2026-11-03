# World Happiness Report 2019 - Statistical EDA & Econometric Analysis

[![Python](https://img.shields.io/badge/Python-3.9%20%7C%203.10%20%7C%203.11-3776AB.svg?logo=python&logoColor=white)](https://www.python.org/)
[![Pandas](https://img.shields.io/badge/Pandas-2.x-150458.svg?logo=pandas&logoColor=white)](https://pandas.pydata.org/)
[![Matplotlib](https://img.shields.io/badge/Matplotlib-3.7+-11557c.svg?logo=matplotlib&logoColor=white)](https://matplotlib.org/)
[![Seaborn](https://img.shields.io/badge/Seaborn-0.12+-4C72B0.svg?logo=seaborn&logoColor=white)](https://seaborn.pydata.org/)
[![Jupyter](https://img.shields.io/badge/Jupyter-Notebook-orange.svg?logo=jupyter&logoColor=white)](https://jupyter.org/)
[![License: MIT](https://img.shields.io/badge/License-MIT-green.svg)](LICENSE)

An in-depth empirical Exploratory Data Analysis (EDA) of the United Nations World Happiness Report (2019) across 156 sovereign states, investigating macroeconomic drivers, social safety nets, institutional trust, and public health metrics correlated with subjective well-being.

---

## Project Overview

National progress has historically been quantified exclusively through Gross Domestic Product (GDP). However, macroeconomic growth metrics fail to capture mental health, community resilience, governance integrity, and individual self-determination.

The **World Happiness Report** shifts policy focus to subjective well-being using the Gallup World Poll's Cantril Ladder life evaluation scores. This project conducts a systematic statistical and exploratory data investigation into the socioeconomic factors underlying national happiness distributions across 156 nations.

### Problem Statement
- **GDP Disconnect**: Pure economic output (GDP per capita) does not guarantee high civic well-being without robust social infrastructure and public health.
- **Multicollinearity in Quality of Life**: Quantifying the individual contributions of health expectancy, governance trust, and civil liberties requires isolated bivariate and multivariate correlation analyses.
- **Outlier Dynamics**: Uncovering outlier nations where high happiness persists despite moderate economic indicators (Nordic social model vs. resource-rich states).

---

## Statistical Correlation Findings

Pearson linear correlation coefficients ($r$) against the Cantril Ladder Happiness Score (`Score`):

| Socioeconomic Determinant | Correlation Coefficient ($r$) | Statistical Significance | Policy Implication |
| :--- | :--- | :--- | :--- |
| **GDP per capita** | **+0.7939** | Strongest Linear Predictor | Economic productivity forms the foundational material threshold |
| **Healthy life expectancy** | **+0.7799** | Highly Positive | Longevity and healthcare access strongly correlate with life satisfaction |
| **Social support** | **+0.7771** | Highly Positive | Informal safety nets and family/community trust act as emotional buffers |
| **Freedom to make life choices** | **+0.5667** | Moderate Positive | Civil liberty and career mobility contribute meaningfully |
| **Generosity** | **+0.0758** | Weak Linear Predictor | Charitable donations show low direct linear linkage to national ranks |
| **Perceptions of corruption** | **+0.3856** | Moderate Non-Linear | Low corruption perception creates an essential stability ceiling |

---

## Top 10 Sovereign Nations Benchmark (2019)

| Rank | Country | Happiness Score | GDP per capita | Social Support | Healthy Life Expectancy |
| :---: | :--- | :---: | :---: | :---: | :---: |
| **1** | Finland | **7.769** | 1.340 | 1.587 | 0.986 |
| **2** | Denmark | **7.600** | 1.383 | 1.573 | 0.996 |
| **3** | Norway | **7.554** | 1.488 | 1.582 | 1.028 |
| **4** | Iceland | **7.494** | 1.380 | 1.624 | 1.026 |
| **5** | Netherlands | **7.488** | 1.396 | 1.522 | 0.999 |
| **6** | Switzerland | **7.480** | 1.452 | 1.526 | 1.052 |
| **7** | Sweden | **7.343** | 1.387 | 1.487 | 1.009 |
| **8** | New Zealand | **7.307** | 1.303 | 1.557 | 1.026 |
| **9** | Canada | **7.278** | 1.365 | 1.505 | 1.039 |
| **10** | Austria | **7.246** | 1.376 | 1.475 | 1.016 |

---

## EDA Workflow Architecture

```
[ UN World Happiness Dataset (2019.csv - 156 Nations) ]
                         │
                         ▼
        [ Data Cleaning & Schema Normalization ]
         ├── Column Renaming & Type Validation
         └── Missing Value & Outlier Inspection
                         │
                         ▼
       [ Descriptive & Distributional Statistics ]
         ├── Parametric Summary Statistics (mean, std, quartiles)
         └── Parametric Dispersion & Histogram Analysis
                         │
                         ▼
        [ Bivariate & Multivariate Analytics ]
         ├── Scatter Plot Regressions (GDP vs Score, Health vs Score)
         └── Pearson & Spearman Correlation Heatmap Calculations
                         │
                         ▼
           [ Econometric Policy Insights ]
         └── Nordic Social Capital Buffering & Governance Trust
```

---

## Project Structure

```
World-Happiness-Report-2019-EDA/
├── World_Happiness_Report_EDA.ipynb   # Complete statistical analysis notebook
├── 2019.csv                           # UN World Happiness Report data (156 countries)
├── requirements.txt                   # Pinned Python dependencies
├── .gitignore                         # Checkpoints, bytecode, and cache exclusions
└── README.md                          # Comprehensive documentation
```

---

## Getting Started

### Prerequisites

- Python 3.9, 3.10, or 3.11
- pip package manager

### Installation & Execution

1. **Clone the repository:**
   ```bash
   git clone https://github.com/pratapashanmukhi/World-Happiness-Report-2019-EDA.git
   cd World-Happiness-Report-2019-EDA
   ```

2. **Create and activate a virtual environment:**
   ```bash
   # Windows:
   python -m venv venv
   .\venv\Scripts\activate

   # Linux / macOS:
   python3 -m venv venv
   source venv/bin/activate
   ```

3. **Install dependencies:**
   ```bash
   pip install -r requirements.txt
   ```

4. **Launch Jupyter Notebook:**
   ```bash
   jupyter notebook World_Happiness_Report_EDA.ipynb
   ```

---

## Author

**Shanmukhi Pratapa**  
B.Tech Computer Science & Engineering (Artificial Intelligence & Machine Learning)  
VIT-AP University  
GitHub: [@pratapashanmukhi](https://github.com/pratapashanmukhi)

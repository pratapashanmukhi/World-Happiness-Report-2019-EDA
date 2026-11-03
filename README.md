# World Happiness Report 2019 — Statistical EDA & Econometric Analysis

[![Python](https://img.shields.io/badge/Python-3.9+-3776AB.svg?logo=python&logoColor=white)](https://www.python.org/)
[![Pandas](https://img.shields.io/badge/Pandas-2.x-150458.svg?logo=pandas&logoColor=white)](https://pandas.pydata.org/)
[![Seaborn](https://img.shields.io/badge/Seaborn-Data%20Viz-4C72B0.svg)](https://seaborn.pydata.org/)
[![License: MIT](https://img.shields.io/badge/License-MIT-green.svg)](LICENSE)

An in-depth statistical Exploratory Data Analysis (EDA) of the United Nations World Happiness Report (2019) surveying 156 nations, investigating macroeconomic determinants, social safety nets, and governance metrics correlated with perceived national well-being.

---

## Dataset Dimensions & Variables (`2019.csv`)

| Variable | Type | Econometric Interpretation |
| :--- | :--- | :--- |
| **Overall rank** | Integer | Global national happiness ranking (1 to 156) |
| **Country or region** | Categorical | Sovereign state surveyed |
| **Score** | Continuous | Cantril Ladder subjective well-being score (0 to 10) |
| **GDP per capita** | Continuous | Purchasing power parity (PPP) adjusted economic output |
| **Social support** | Continuous | Perceived availability of assistance during personal hardship |
| **Healthy life expectancy** | Continuous | Years of healthy physical life projected at birth |
| **Freedom to make life choices** | Continuous | Perceived autonomy in personal and professional choices |
| **Generosity** | Continuous | Charitable donations adjusted for national wealth |
| **Perceptions of corruption** | Continuous | Institutional trust in business and governmental authorities |

---

## Key Analytical Insights

1. **Dominant Macroeconomic Correlation**: `GDP per capita` ($r \approx 0.79$) and `Healthy life expectancy` ($r \approx 0.78$) exhibit the strongest positive linear correlation with national happiness scores.
2. **Social Capital Buffer**: `Social support` acts as a crucial resilience multiplier; nations with moderate GDP but high social trust frequently outrank wealthier nations with fragmented social cohesion.
3. **Corruption Non-Linearity**: High perception of institutional corruption correlates with a severe ceiling on subjective well-being scores.

---

## Project Structure

```
World-Happiness-Report-2019-EDA/
├── World_Happiness_Report_EDA.ipynb   # Complete statistical analysis notebook
├── 2019.csv                           # UN World Happiness Report data (156 countries)
├── requirements.txt                   # Dependency declarations
├── .gitignore                         # Build and notebook cache exclusions
└── README.md                          # Technical documentation
```

---

## Installation & Execution

```bash
git clone https://github.com/pratapashanmukhi/World-Happiness-Report-2019-EDA.git
cd World-Happiness-Report-2019-EDA
python -m venv venv
source venv/bin/activate  # or .\venv\Scripts\activate on Windows
pip install -r requirements.txt
jupyter notebook World_Happiness_Report_EDA.ipynb
```

---

## Author

**Shanmukhi Pratapa**  
B.Tech CSE (AI & ML) — VIT-AP University  
GitHub: [@pratapashanmukhi](https://github.com/pratapashanmukhi)

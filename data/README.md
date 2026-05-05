# California Mental Health Services — Exploratory Data Analysis

**Author:** Kesheka Edupuganti | [Portfolio](https://keportfolio.vercel.app) | [LinkedIn](https://linkedin.com/in/kesheka-edupuganti-b53a96293)

---

## Overview

California spends billions on mental health services every year. But who is actually being served? Are the right people getting access? And which counties are being left behind?

This project explores four years of adult mental health service utilization data across all California counties using Python, Pandas, Seaborn and Matplotlib.

---

## Key Findings

- Adult beneficiaries grew from 13.6M to 16.4M service contacts between FY2019-20 and FY2022-23, a 20.8% increase
- Utilization grew every year including through COVID-19, likely driven by telehealth expansion and Medi-Cal eligibility changes
- Los Angeles alone accounts for more beneficiaries than the next 5 counties combined. Alpine county has just 100 served — a 37,000x gap
- Hispanic and White adults represent the largest beneficiary groups, reflecting California demographics
- Female beneficiaries account for 60.8% of all adults served
- Working-age adults (21-32) are the most served age group
- NSMHS (Non-Specialty) services grew significantly faster than SMHS (Specialty) over the study period

---

## Charts

| Chart | Description |
|-------|-------------|
| 01_statewide_trends.png | Total adult beneficiaries and year-over-year growth by fiscal year |
| 02_county_analysis.png | Top 20 and bottom 20 counties by total beneficiary count |
| 03_demographics.png | Breakdown by sex, race/ethnicity and age group |
| 04_county_trends.png | Top 10 county trajectories over time |
| 05_delivery_system.png | SMHS vs NSMHS beneficiary comparison over time |

---

## Data Source

All data is sourced from the **California Health and Human Services Open Data Portal**.

Dataset: [Behavioral Health Program Performance Data](https://data.chhs.ca.gov/dataset/behavioral-health-program-performance-data)

Download these four CSV files and place them in the same folder as the notebook before running:

| Filename to use | File to download from CHHS |
|-----------------|---------------------------|
| `adult_utilization_by_sex.csv` | Adult SMHS and MHS Service Utilization Data by Sex |
| `adult_utilization_by_race.csv` | Adult SMHS and MHS Service Utilization Data by Race |
| `adult_utilization_by_age.csv` | Adult SMHS and MHS Service Utilization Data by Age |
| `all_demo_data_new_3.csv` | Demographic Data for FY's 2020-2023 |

Note: The demographic file requires `encoding='latin-1'` and `engine='python'` when loading with Pandas.

---

## Tools

Python, Pandas, NumPy, Matplotlib, Seaborn

---

## How to Run

```bash
git clone https://github.com/KeshekaE/ca-mental-health-eda
cd ca-mental-health-eda
pip install pandas numpy matplotlib seaborn
# Download the four CSVs from CHHS and place in this folder
jupyter notebook CA_Mental_Health_EDA.ipynb
```

---

*This project is part of my data analytics portfolio. Next step: building a county-level KPI dashboard in Power BI using this same dataset.*

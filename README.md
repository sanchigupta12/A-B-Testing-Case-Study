# Simulating Real-World A/B Testing Data with Imperfections

## Project Overview

This project simulates an A/B testing scenario to evaluate user engagement between two webpage versions — **Control** and **Experimental** — with **Click-Through Rate (CTR)** as the key performance metric.

To reflect real-world data challenges, the project introduces:
- Missing values
- Inconsistent labels
- Duplicates
- Outliers

This makes it a **realistic case study** for applying data cleaning, transformation, and statistical testing techniques used by **Data Analysts**, **Data Engineers**, and **Product Analysts** in production environments.

---

## Tools & Libraries
- **Python** (Pandas, NumPy, Matplotlib, Seaborn, SciPy, StatsModels)
- **Jupyter Notebook**
- **A/B Testing Concepts**
- **Z-Test**, Confidence Intervals, and Practical Significance Analysis

---

## Simulated Data
We generated a dataset of 200K+ records simulating:
- Binary click outcomes (`click`)
- Group assignment (`exp`, `con`)
- Session time
- Click timestamp
- Device type (mobile/desktop)
- Referral sources (email, social, search, etc.)

Real-world data imperfections were injected to emulate:
- Logging errors (nulls)
- Data entry issues (label casing, typos)
- ETL bugs (duplicates)
- Tracking anomalies (outliers)

---

## Data Cleaning Highlights
- **Handled nulls** in critical columns (click time, group)
- **Standardized labels** (lowercase, strip whitespace)
- **Dropped duplicates**
- **Identified and removed session time outliers** using IQR filtering

---

## Exploratory Data Analysis
- CTR distributions across `group`, `device_type`, and `referral_source`
- Time-based click trends
- Bar plots and boxplots for CTR comparisons

---

## Statistical Analysis
- One-tailed **Z-Test** to test:
  - **H₀**: No difference in CTR between groups
  - **H₁**: Experimental group has higher CTR
- **P-value < 0.05** → Statistically significant
- **95% Confidence Interval** confirms improvement
- **Minimum Detectable Effect (MDE)** of 5% passed → Practically significant

---

## Results

- **CTR (Experimental):** ~50%  
- **CTR (Control):** ~20%  
- **Z-Statistic:** 133.75  
- **P-Value:** 0.0000  
- **95% CI:** [0.294, 0.302]  
- Both **statistical** and **practical** significance were achieved.

---

## Visualizations Included
- CTR breakdowns by group, device, and referral source
- Daily click volume
- Z-distribution plot highlighting test statistic and critical threshold




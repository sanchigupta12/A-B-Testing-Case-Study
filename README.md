# A/B Testing Case Study – Simulated Clickstream Data

This project demonstrates a complete A/B testing workflow using simulated clickstream data to analyze user engagement across two webpage designs — Control and Experimental groups. The goal is to determine if the new design leads to a statistically and practically significant improvement in click-through rates (CTR).

---

## Key Objectives

- Simulate user click data for A/B groups
- Visualize group-wise CTR distribution
- Perform Two-Sample Z-Test for statistical significance
- Calculate Confidence Interval and P-value
- Evaluate **practical significance** using Minimum Detectable Effect (MDE)
- Visualize standard normal curve with rejection regions

---

## Key Concepts Covered

- Hypothesis Testing (Two-Tailed Z-Test)
- Confidence Interval Interpretation
- P-Value Analysis
- Practical vs Statistical Significance
- Standard Normal Distribution & Rejection Regions

---

## Tools & Libraries

- Python (Pandas, NumPy, Matplotlib, Seaborn, SciPy)
- Jupyter Notebook / Google Colab

---

## Project Outcome

- The experimental group showed a **higher CTR** than the control group.
- Results were **statistically significant** (p < 0.05).
- Results were also **practically significant** with a meaningful improvement above the business-defined threshold (MDE).

---

## File Structure
| File                             | Description                               |
|----------------------------------|-------------------------------------------|
| `AB_Testing_Case_Study.ipynb`    | Full A/B test notebook with code & plots  |
| `README.md`                      | Project overview and documentation        |

---

## How to Run

1. Clone this repo:
```bash
git clone https://github.com/your-username/ab-testing-ctr-case-study.git

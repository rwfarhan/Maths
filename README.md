# 📊 Employee Performance — Mathematical Analysis

A hands-on data analysis project applying core mathematical and statistical concepts to a real-world employee performance dataset (4,000 records).

---

## 📁 Repository Contents

| File | Description |
|------|-------------|
| `exam_solution.ipynb` | Main Jupyter notebook with all analysis and code |
| `employee_performance.csv` | Dataset — 4,000 employee records |
| `analysis_plots.png` | Exported visualizations |
| `exam_report.docx` | Written exam report |

---

## 🗂️ Dataset Overview

The dataset contains **4,000 employee records** with the following features:

| Column | Description |
|--------|-------------|
| `Employee_ID` | Unique identifier |
| `Age` | Employee age (22–59) |
| `Salary` | Annual salary (₹25,000–₹98,193) |
| `Department` | Finance, HR, IT, Marketing, Operations |
| `Projects_Completed` | Number of projects completed (0–16) |
| `Working_Hours` | Weekly working hours (20–73.1) |
| `Performance_Score` | Score out of 100 (11.7–100) |
| `Promotion_Status` | Whether the employee was promoted (Yes/No) |

---

## 🔬 Analysis Breakdown

### 1 — Central Tendency & Dispersion
- **Mean, Median, Mode** of Salary
- **Variance and Standard Deviation** of Projects Completed

### 2 — Probability & Events
- Overall promotion probability: **P(Promotion) = 49.45%**
- Contingency table of Promotion Status vs Department
- Conditional probability: **P(Promotion | Score > 80) = 59.16%**

### 3 — Distributions & Visualization
- Histogram of Performance Score overlaid with a Gaussian curve
- Skewness and Kurtosis analysis for Salary and Performance Score
- Q-Q Plot for Projects Completed to test for normality

### 4 — Linear Algebra Application
- Employee work profiles represented as 2D vectors `[Projects_Completed, Working_Hours]`
- **Dot product** to measure similarity between employees
- **L1 (Manhattan) and L2 (Euclidean) norms**
- **Cosine angle** between employee vectors to determine working-style similarity

---

## 💡 Key Findings

1. Employees with Performance Score > 80 have a **59.2% promotion chance** — significantly higher than the overall rate.
2. **Marketing** has the highest promotion rate at **51.2%**.
3. Average salary is **₹54,979**, with near-zero skewness (0.050) indicating a balanced pay scale.
4. Only **15.4%** of employees score above 80 — high performers are rare.
5. Projects Completed follows a **Poisson-like distribution**, not a Normal one (confirmed via Q-Q plot, r = 0.9845 with visible deviation at tails).

---

## 🛠️ Tech Stack

- **Python 3**
- `pandas` — data manipulation
- `numpy` — numerical computing & linear algebra
- `matplotlib` — visualization
- `scipy.stats` — statistical distributions & tests

---

## 🚀 Getting Started

```bash
git clone https://github.com/rwfarhan/Maths.git
cd Maths
pip install pandas numpy matplotlib scipy
jupyter notebook exam_solution.ipynb
```

---

## 👤 Author

**rwfarhan** — [github.com/rwfarhan](https://github.com/rwfarhan)

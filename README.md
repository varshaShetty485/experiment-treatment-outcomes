# Experimentation on Treatment Outcomes (Simulated A/B Test)

This project simulates and analyzes clinical trial data to evaluate the effectiveness of two medical treatments (Treatment A and Treatment B) compared to a Control group. The goal is to determine if observed differences in recovery time are statistically and practically significant.

---

##  Project Overview

- **Objective**: Determine whether Treatment A or B leads to significantly faster recovery than the Control group.
- **Approach**: Simulate clinical data and apply statistical hypothesis testing using t-tests, ANOVA, and post-hoc analysis.
- **Tools Used**: Python, NumPy, pandas, SciPy, Statsmodels, Matplotlib, Seaborn

---

## Methods and Analysis

### 1. Data Simulation
- Created synthetic data for 3 patient groups (n = 100 per group)
  - **Control**: Standard treatment
  - **Treatment A**: Moderate improvement
  - **Treatment B**: Strong improvement
- Simulated recovery times using normal distributions

### 2. Statistical Assumption Checks
-  **Shapiro-Wilk test**: Confirmed normal distribution in each group  
-  **Levene’s test**: Confirmed equal variances across groups

### 3. Hypothesis Testing
- **One-Way ANOVA**: p-value < 0.00001 → Significant differences found between groups
- **Tukey’s HSD**: All pairwise group differences were statistically significant

### 4. Confidence Intervals & Effect Sizes
- 95% Confidence Intervals calculated for mean recovery times
- **Cohen's d** effect sizes:
  - Control vs Treatment A: 0.40 (small-medium)
  - Control vs Treatment B: 0.83 (**large**)
  - Treatment A vs B: 0.45 (medium)

---

##  Visualizations

- **Boxplot**: Shows recovery time distributions across groups
- **Bar chart with 95% CI**: Highlights average treatment effects and uncertainty



##  Conclusion

- Both Treatment A and Treatment B significantly improve recovery time over the Control.
- Treatment B is the most effective, showing a large and practically meaningful impact.
- Statistical analysis supports strong evidence for adopting Treatment B in clinical decision-making (based on this simulation).

---

## Technologies Used

| Tool       | Purpose                         |
|------------|----------------------------------|
| Python     | Programming language             |
| NumPy      | Random number generation         |
| pandas     | Data manipulation                |
| SciPy      | Hypothesis testing (t-test, Levene's, Shapiro-Wilk) |
| Statsmodels | ANOVA, Tukey HSD                |
| Matplotlib & Seaborn | Visualization          |
| Google Colab | Development environment        |

---





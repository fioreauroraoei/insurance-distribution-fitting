# Claim Severity Analysis — Actuarial Data Analytics Project

This project was originally developed as part of my **Data Analytics for Actuarial Science** coursework.  
It has been adapted and expanded into a portfolio project to demonstrate my ability in **data cleaning**, **distribution fitting**, and **actuarial interpretation**.

---

## Project Overview
Insurance claim amounts often display **skewed and heavy-tailed** characteristics, making accurate modeling essential for pricing and risk management.  
This project explores several probability distributions — **Lognormal, Gamma, Weibull, and Pareto** — to identify the most appropriate model for insurance claim severity data.

The analysis includes:
- Exploratory Data Analysis (EDA)
- Parameter estimation via Maximum Likelihood Estimation (MLE)
- Model selection using AIC/BIC and goodness-of-fit tests
- Tail risk evaluation using VaR and TVaR
- Sensitivity analysis for model robustness

---

## Methodology

### **1. Exploratory Data Analysis**
- Loaded `claim_severity.csv`
- Computed descriptive statistics: mean, median, standard deviation, skewness, kurtosis
- Created histogram (log-scale), empirical CDF, and mean excess plot
- Diagnosed tail heaviness

### **2. Parametric Fitting via MLE**
- Fitted candidate distributions: Lognormal, Gamma, Weibull, Pareto
- Estimated parameters and confidence intervals
- Visualized fitted densities over histogram

### **3. Model Adequacy & Selection**
- Compared log-likelihood, AIC, and BIC
- Conducted goodness-of-fit diagnostics (QQ-plots, KS/AD tests)
- Selected the most suitable distribution and justified the choice

### **4. Tail Risk & Pricing**
- Computed Value-at-Risk (VaR) and Tail Value-at-Risk (TVaR) at 95% and 99% confidence levels
- Interpreted results in the context of insurance pricing and capital requirements

### **5. Sensitivity Check**
- Truncated top 1% of claims
- Re-fitted the selected distribution
- Evaluated stability of fitted parameters and tail measures

---

## Tools & Libraries
- **Python**: pandas, numpy, scipy.stats, matplotlib, seaborn
- **Jupyter Notebook** for analysis and documentation
- **Statistical fitting** using Maximum Likelihood Estimation
- **Goodness-of-fit tests** (Kolmogorov–Smirnov, Anderson–Darling)

---

## Key Insights
- Claim severity data shows strong **right-skewness** and **heavy tails**.  
- **Lognormal** and **Pareto** distributions gave the best fits depending on tail emphasis.  
- Tail measures (VaR/TVaR) highlight substantial potential losses, supporting the need for robust capital management.

---

## Project Structure
 claim-severity-analysis/
│
├── claim_severity.csv             # Raw dataset
├── claim_severity_analysis.ipynb  # Main notebook
├── README.md                      # Project description (this file)
└── outputs/
    ├── fitted_distributions.png
    ├── qq_plots.png
    └── tail_metrics_summary.pdf


[![Review Assignment Due Date](https://classroom.github.com/assets/deadline-readme-button-22041afd0340ce965d47ae6ef1cefeee28c7c493a6346c4f15d667ab976d596c.svg)](https://classroom.github.com/a/QaCpgAB-)
Assignment 2 – Fit & Interpret Probability

Distributions for Claim Severity
**Course:** Data Analytics for Actuarial Science
**Week:** 5
**Dataset:** claim_severity.csv (column: claim_amount)
**Deliverables:** Notebook + brief PDF summary + figures (Use proper naming format e.g. std_number-file_name-assignment2.ipynb)

Learning Objectives
• Diagnose heavy-tailed behavior in claim severities.
• Fit candidate severity distributions (Lognormal, Gamma, Weibull, Pareto).
• Compare models using information criteria and goodness-of-fit diagnostics.
• Compute tail risk measures (VaR/TVaR) and interpret actuarially.

Part A — Exploratory Data Analysis (EDA) (10 pts)
• Load claim_severity.csv and report: sample size n, mean, median, std, coefficient of variation,
skewness, kurtosis.
• Plot: histogram (density-scaled) with log-x, empirical CDF, and mean excess plot.
• Write 2–3 sentences diagnosing tail heaviness.

Part B — Parametric Fits via MLE (30 pts)
• Fit Lognormal, Gamma, Weibull, and Pareto using MLE.
• Report parameter estimates and standard errors (or bootstrap CIs).
• Overlay fitted densities on histogram (log-x).

Part C — Model Adequacy & Selection (30 pts)
• Compute log-likelihood, AIC, and BIC. Rank models.
• Goodness-of-fit: QQ-plots, KS and/or AD tests.
• Select a preferred model and justify.

Part D — Tail Risk & Pricing (20 pts)
• For preferred model, compute VaR95, VaR99, TVaR95, TVaR99.
• Interpret tail measures for pricing and capital.

Part E — Sensitivity Check (10 pts)
• Truncate top 1% of claims and refit preferred model.
• Compare parameters and VaR/TVaR; discuss robustness.

Bonus (+5 pts)
Fit a truncated Lognormal or mixture (e.g., 2-component Lognormal) and compare AIC/BIC.
Grading Rubric (100 pts)
• EDA: 10
• Fits: 30
• Selection: 30
• Tail risk: 20
• Sensitivity: 10
• Bonus: +5

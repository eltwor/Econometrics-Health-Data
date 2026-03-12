# Blood Pressure Regression Analysis

This project was completed as part of my Econometrics coursework at the University of Rzeszów. It demonstrates my ability to apply statistical modeling techniques to real-world health data—a skill directly transferable to data-driven roles in FinTech and beyond.

## Objective

To model systolic blood pressure using various health and lifestyle indicators (weight, height, BMI, waist circumference, age, diabetes, smoking, fast food consumption). I built and compared four regression models, selecting variables based on correlation analysis and diagnostic plots.

## Key Steps

1. **Data Exploration** – Summary statistics, histograms, and correlation matrix to understand variable distributions and relationships.
2. **Model Building** – Constructed four models:
   - Simple linear regression (systolic ~ age)
   - Multiple linear regression (systolic ~ age + weight, age + waist)
   - Polynomial regression (systolic ~ age + age²)
   - Binary variable regression (systolic ~ smoker, systolic ~ diabetes)
3. **Model Comparison** – Used adjusted R², AIC/BIC, and F-tests to evaluate performance.
4. **Residual Diagnostics** – Tested for normality (Shapiro-Wilk), homoscedasticity (Breusch-Pagan), autocorrelation (Durbin-Watson), and linearity (RESET test).
5. **Interpretation** – Analyzed coefficient significance and practical implications.

## Tools Used

- **R** – Data manipulation, modeling, and statistical tests.
- **R Markdown** – Dynamic report generation with integrated code and visualizations.
- **Libraries**: `dplyr`, `ggplot2`, `corrplot`, `lmtest`, `broom`, `knitr`.

## Key Findings

- Age was the strongest predictor of systolic blood pressure (positive correlation).
- Variables related to body size (weight, BMI, waist) were highly correlated with each other, so only one was used in multiple regression to avoid multicollinearity.
- All models suffered from non-normal residuals, suggesting potential for transformation or more complex modeling.

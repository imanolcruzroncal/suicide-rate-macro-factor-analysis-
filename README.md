# Global Suicide Rate Analysis Using Macroeconomic and Social Indicators

## Overview

This project analyzes the macro-level factors associated with suicide rates across countries using a country-year panel dataset. The analysis integrates economic, social, and health indicators from international databases and applies econometric models to identify patterns and relationships that influence suicide rates globally.

The objective is to understand how macroeconomic conditions, labor market factors, mental health indicators, and inequality interact with suicide trends across countries and over time.

---

## Research Objective

The main objective of this project is to identify macro-level factors that show consistent relationships with suicide rates using data science techniques and statistical analysis.

Specifically, the project aims to:

- Build a global dataset integrating economic, social, and health indicators
- Analyze suicide trends across countries and years
- Identify macroeconomic and social determinants of suicide rates
- Apply panel data econometric models to evaluate relationships between variables

---

## Data Sources

The dataset integrates multiple international sources:

- World Health Organization (WHO)
- World Bank – World Development Indicators
- Institute for Health Metrics and Evaluation (IHME)
- International Labour Organization (ILO)
- Transparency International

These sources provide standardized global indicators that allow cross-country comparisons.

---

## Dataset Structure

The project builds a **country-year panel dataset**, where each row represents a specific country in a specific year.

Main variables included:

### Dependent Variable

- Suicide rate

### Economic Indicators

- GDP per capita (PPP)
- Unemployment rate
- Inflation

### Inequality Indicators

- GINI index
- Poverty rate

### Labor Market Indicators

- Labor force participation
- Informal employment

### Education Indicators

- Literacy rate
- Tertiary education enrollment

### Health Indicators

- Depression prevalence
- Drug use disorder prevalence
- Alcohol consumption

### Institutional Indicators

- Corruption perception index
- Homicide rate

---

## Data Engineering Workflow

The dataset required extensive data preparation and integration:

1. Data collection from multiple international sources
2. Cleaning and standardizing country names
3. Converting datasets from wide format to long format
4. Handling missing values and data coverage differences
5. Interpolating small internal missing gaps
6. Merging datasets using country and year as keys
7. Building a master country-year panel dataset

Python and reproducible scripts were used to ensure transparency and repeatability.

---

## Methodology

The analysis uses **panel data econometrics** to examine relationships between suicide rates and macro factors.

### Model 1 – Baseline Model

Ordinary Least Squares (OLS) regression analyzing relationships between:

- Depression prevalence
- Drug use disorders
- Alcohol consumption

### Model 2 – Fixed Effects Model

Panel regression including:

- Country fixed effects
- Year fixed effects

This model controls for:

- Cultural differences across countries
- Structural national characteristics
- Global shocks affecting all countries simultaneously

### Model 3 – Macroeconomic Expansion

Additional macroeconomic variables included:

- GDP per capita
- Unemployment
- Inflation

### Model 4 – Structural Factors

Final models incorporate structural indicators such as:

- Income inequality
- Poverty
- Education indicators

Clustered standard errors were used to improve statistical robustness.

---

## Key Findings

Several consistent patterns emerge from the analysis:

- Higher GDP per capita is associated with lower suicide rates
- Higher unemployment is associated with higher suicide rates
- Depression prevalence shows a positive association with suicide rates
- Drug and alcohol consumption show positive associations in some models
- Income inequality does not show strong short-term effects within countries

Overall, **economic conditions and labor market stability appear to be key structural determinants of suicide rates.**

---

## Tools and Technologies

Python  
Pandas  
NumPy  
Jupyter Notebook  
Panel Data Econometrics  
Statistical Modeling  

---

---

## Limitations

Some limitations are inherent to international macro-level datasets:

- Missing data across countries and years
- Differences in data collection methodologies
- Limited coverage for some indicators
- Unbalanced panel dataset

Despite these limitations, the dataset provides valuable insights into global patterns.

---

## Future Work

Future improvements could include:

- Machine learning models for suicide risk prediction
- Regional cluster analysis
- Additional social and behavioral indicators
- Interactive dashboards for visualization

---

## Author

Abraham Imanol Cruz Roncal

Industrial Engineer  
Master of Science in Engineering Management  

Research interests:

- Data Science
- Econometrics
- Public Health Analytics
- Global Development Analysis

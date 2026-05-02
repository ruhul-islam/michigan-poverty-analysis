# Michigan Poverty Analysis: What Drives Poverty Across Michigan Counties?

**Author:** Ruhul Islam  
**Tools:** Tableau, Census Data (2015)  
**Published:** December 2025  
**Tableau Public:** [View Interactive Dashboards](https://public.tableau.com/app/profile/ruhul.islam/vizzes)

---

## Overview

This project analyzes poverty patterns across all 83 Michigan counties using 2015 US Census data. The goal was to identify the strongest predictors of county-level poverty rates and understand whether Michigan's poverty challenge is primarily a jobs problem or a wages problem.

**Key Finding:** Median household income is a significantly stronger predictor of poverty (R² = 0.51) than unemployment rate (R² = 0.32). This suggests Michigan's poverty challenge is more about low wages than lack of employment.

---

## Visualizations

### 1. Geographic Distribution of Poverty Across Michigan Counties
[View on Tableau Public](https://public.tableau.com/app/profile/ruhul.islam/viz/GeographicDistributionofPovertyAcrossMichiganCounties/GeographicDistributionofPovertyAcrossMichiganCounties)

A choropleth map showing poverty rates across all 83 Michigan counties. Key patterns:
- Highest poverty (20-30%) concentrated in the Upper Peninsula and northern rural counties
- Lowest poverty (under 10%) in Detroit suburbs, Grand Rapids, and Ann Arbor metro areas
- Interactive income filter allows exploration of how poverty shifts across income thresholds

**Design decisions:** White-to-red color scheme for intuitive severity mapping, colorblind-accessible palette, automatic labeling of counties exceeding 20% poverty threshold.

---

### 2. Income Strongly Predicts Poverty in Michigan Counties (R² = 0.51)
[View on Tableau Public](https://public.tableau.com/app/profile/ruhul.islam/viz/IncomeStronglyPredictsPovertyinMichiganCountiesR0_51/IncomeStronglyPredictsPovertyinMichiganCountiesR0_51)

A scatter plot showing the relationship between median household income and poverty rate across Michigan counties.
- Trend line with R² = 0.51 confirms income as the primary predictor
- Dots colored by unemployment rate reveal that worst-off counties typically have both low income and high unemployment
- Dot size scaled by population to highlight larger counties
- Isabella County identified as an outlier — higher poverty than income would predict, likely driven by its large student population

---

### 3. What Drives Poverty in Michigan? (Dashboard)
[View on Tableau Public](https://public.tableau.com/app/profile/ruhul.islam/viz/WhatDrivesPovertyinMichigan/WhatDrivesPovertyinMichigan)

A comparative dashboard contrasting high-poverty counties (poverty rate above 20%) against low-poverty counties (poverty rate below 10%).

| Metric | High Poverty Counties | Low Poverty Counties |
|---|---|---|
| Median Household Income | $39,000 | $72,000 |
| Professional Jobs | 28% | 40% |
| Service Jobs | 22% | 15% |
| Unemployment Rate | 12% | 6% |

**Design decisions:** Income and employment metrics separated into distinct bar charts due to incompatible scales. Interactive scatter plot allows click-through exploration of individual county data.

---

## Key Takeaways

1. **Income matters more than employment.** The data shows Michigan's poverty challenge is structural — it is about job quality, not job availability.

2. **Geography reflects job concentration.** Professional employment clusters around major cities. Rural and northern communities face a shortage of living-wage opportunities, not a shortage of workers.

3. **49% of variance remains unexplained.** Income alone does not tell the whole story. Education levels, cost of living differences, and family structure likely account for significant remaining variation — factors not captured in this dataset.

4. **Policy implication.** Addressing Michigan's poverty gap requires expanding access to professional employment in rural communities, not simply increasing low-wage service sector jobs.

---

## Data Source

- US Census Bureau American Community Survey (ACS) 2015 5-Year Estimates
- County-level data for all 83 Michigan counties
- Variables: median household income, poverty rate, unemployment rate, employment by industry

---

## Repository Structure
michigan-poverty-analysis/
├── README.md
├── data/
│   └── michigan_counties_2015.csv
└── analysis/
└── michigan_poverty_report.pdf

---

## Connect

- **Tableau Public:** [ruhul.islam](https://public.tableau.com/app/profile/ruhul.islam/vizzes)
- **GitHub:** [github.com/ruhul-islam](https://github.com/ruhul-islam)
- **LinkedIn:** linkedin.com/in/ruhulislam

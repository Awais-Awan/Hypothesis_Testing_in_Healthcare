# Drug Safety Data Analysis Project

This repository contains a project that analyzes drug safety data, focusing on comparing the incidence of adverse effects between patients in two groups: those receiving a drug and those receiving a placebo. The analysis employs several statistical methods to determine significant differences between the groups, along with visualizing the data.

## Project Overview

In this project, we analyzed the adverse effects experienced by patients in a clinical trial. The goal was to understand if the drug had a higher likelihood of causing adverse effects compared to a placebo, while also exploring other factors such as age and the number of effects.

### Key Steps:

1. **Data Loading**: The dataset (`drug_safety.csv`) was loaded into a Pandas DataFrame for analysis.
2. **Adverse Effects Comparison**: The incidence of adverse effects was compared between the drug and placebo groups using a **two-proportion Z-test**.
3. **Chi-Squared Test**: We tested the independence between the number of effects and the treatment group using a **Chi-squared test**.
4. **Age Distribution**: Visualized the age distribution in both groups using a **Seaborn histogram**.
5. **Normality Testing**: Applied a **Shapiro-Wilk test** to assess the normality of the age data.
6. **Non-parametric Testing**: Since the data distribution was non-normal, we used a **Mann-Whitney U test** to compare the age distributions.

## Results

- The two-proportion Z-test revealed whether the proportion of adverse effects significantly differed between the drug and placebo groups.
- The Chi-squared test showed the relationship between the number of adverse effects and the treatment group.
- The Mann-Whitney U test compared the age distributions, as the normality assumption was violated.

## Visualizations

- A **histogram** showing the age distribution across the two groups (drug and placebo) was generated using Seaborn.

## Technologies

- **Python**: Primary language used.
- **Pandas**: For data manipulation and analysis.
- **NumPy**: To handle numerical operations.
- **Statsmodels**: For performing the two-proportion Z-test.
- **Pingouin**: Used for statistical testing like the Chi-squared test, normality test, and Mann-Whitney U test.
- **Seaborn**: For data visualization.
- **Matplotlib**: For plotting graphs.

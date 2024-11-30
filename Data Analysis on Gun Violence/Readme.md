# Exploratory Data Analysis on Gun Violence and Health Insurance Costs

## Author: Prachi Aswani

---

### Overview
This repository contains the analysis and exploration of two datasets related to public health: **Gun Violence Data** and **Health Insurance Costs**. Through various data wrangling, visualization, and statistical techniques, the goal of this analysis is to explore patterns, correlations, and trends that might reveal insights about these pressing social issues. 

The primary focus of the analysis is to answer questions such as:
- How does the Body Mass Index (BMI) of a person impact health insurance costs?
- What trends and correlations can be observed from gun violence incidents across different states and years?

---

### Table of Contents
1. [Data Analysis Questions](#data-analysis-questions)
2. [Data Preparation](#data-preparation)
3. [Exploratory Data Analysis on Health Insurance Costs](#exploratory-data-analysis-on-health-insurance-costs)
4. [Exploratory Data Analysis on Gun Violence](#exploratory-data-analysis-on-gun-violence)
5. [Visualizations](#visualizations)
6. [Statistical Analysis and Hypothesis Testing](#statistical-analysis-and-hypothesis-testing)
7. [Data Ethics Canvas](#data-ethics-canvas)
8. [Conclusion](#conclusion)
9. [Files in this Repository](#files-in-this-repository)

---

### Data Analysis Questions
1. **How does the Body Mass Index (BMI) of a person impact health insurance costs?**
2. **What are the trends in gun violence incidents across the U.S., and how do these vary by state, year, and other factors?**

---

### Data Preparation
The datasets used in this analysis are as follows:
- **Health Insurance Costs Dataset**: Contains information about individuals' demographics (age, sex, BMI, smoking status, etc.) and their respective health insurance charges.
- **Gun Violence Data**: Contains records of gun violence incidents across the U.S., including details like the incident's location, number of casualties, and other attributes.

Data was loaded from a GitHub repository and cleaned for further analysis, including handling missing values, filtering out irrelevant entries, and checking for data consistency.

---

### Exploratory Data Analysis on Health Insurance Costs
In this analysis, the main question is how BMI affects health insurance costs. We performed the following:
- Summary statistics and data validation to understand distributions and potential outliers.
- Visualized relationships between BMI and health insurance charges using regression plots.
- Validated normality of data using normal probability plots.
- Calculated correlation coefficients and performed hypothesis testing to assess the relationship between BMI and charges.

---

### Exploratory Data Analysis on Gun Violence
For the gun violence dataset, the main focus was to explore:
- Trends in gun violence over time.
- The relationship between incidents and demographic factors (such as location).
- Key factors such as the number of casualties (dead and injured) in different states and regions.

---

### Visualizations
Several visualizations were generated to help understand the relationships between the variables:
- **Regressions and Scatter Plots**: Used to assess the linearity between BMI and health insurance costs.
- **Distribution Plots**: To visualize the distribution of charges and BMI across the dataset.
- **Trend Visualizations**: To assess gun violence trends across states and over time.

---

### Statistical Analysis and Hypothesis Testing
We used statistical tools such as:
- **Pearson Correlation Coefficient** to quantify the relationship between BMI and health insurance charges.
- **T-tests and Normality Tests** to validate assumptions and understand the underlying distributions of variables.

---

### Data Ethics Canvas
In all analyses, the **Data Ethics Canvas** was employed to ensure the ethical handling of sensitive data. Key considerations included:
- **Privacy**: Handling personal information such as BMI and health insurance charges with care.
- **Bias**: Checking for and addressing any biases in the data, especially concerning gender, age, and region.
- **Transparency**: Clearly documenting methodologies, assumptions, and potential limitations of the data and analyses.

---

### Conclusion
The exploratory data analysis on both gun violence and health insurance costs reveals valuable insights:
- **Health Insurance Costs**: A weak positive correlation was found between BMI and insurance charges, suggesting that higher BMI may lead to slightly higher costs, although the effect is not strong.
- **Gun Violence Trends**: There are noticeable patterns in gun violence incidents over the years, with varying levels of incidents across different states.


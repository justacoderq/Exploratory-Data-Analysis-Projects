# DS 2500 – Module Assignment 01: Exploratory Data Analysis on Health Insurance Costs
**Author**: Prachi Aswani

---

### **1. Overview**

This project involves performing **Exploratory Data Analysis (EDA)** on a health insurance dataset to explore how various factors like **Body Mass Index (BMI)** impact **Health Insurance Costs**. The analysis investigates the relationship between BMI and health insurance charges, with a particular focus on understanding how personal health metrics influence the cost of healthcare.

---

### **2. Data Analysis Question**
**How does the Body Mass Index (BMI) of a person impact health insurance costs?**

---

### **3. Dataset Description**

The dataset used in this analysis contains various demographic and health-related features of individuals who are insured. Key columns in the dataset include:

- **age**: Age of the individual
- **sex**: Gender of the individual
- **bmi**: Body Mass Index (BMI)
- **children**: Number of children/dependents covered by the insurance
- **smoker**: Whether the individual is a smoker (yes or no)
- **region**: Region of the individual (northwest, southwest, southeast, northeast)
- **charges**: Health insurance charges

The dataset is publicly available and can be accessed directly from GitHub:  
[Insurance Dataset](https://raw.githubusercontent.com/Pauline177/DataScience2500/main/insurance.csv)

---
### **4. Exploratory Data Analysis (EDA)**

The dataset was first loaded into a pandas DataFrame. After inspecting the data and performing basic preprocessing steps, various analyses were conducted to understand the relationship between the variables.

#### **Key Steps in the EDA Process:**

1. **Data Inspection**:
    - The dataset was loaded and the shape of the data was checked, confirming it contains 1338 rows and 7 columns.
    - The top and bottom of the dataset were inspected using `df.head()` and `df.tail()` to understand the structure of the data.

2. **Summary Statistics**:
    - Summary statistics were computed for key variables, especially for `charges`, which represent health insurance costs. This revealed a right-skewed distribution with charges ranging from \$1,121 to \$63,770.

3. **Exploration of Variables**:
    - Frequency distributions of variables like `children`, `smoker`, `region`, and `sex` were examined.
    - The BMI variable was particularly interesting, with 548 unique BMI values suggesting considerable variability in the data.

4. **Data Visualizations**:
    - A **regression plot** was created to explore the relationship between **BMI** and **health insurance charges**. This visual representation helps assess any trends or linear relationships.
    - A **normal probability plot** was generated to assess if the distribution of `charges` follows a normal distribution. Different distributions (Normal, T, and Gamma) were tested to understand the underlying patterns.

---

### **5. Key Findings**

The exploratory data analysis provided valuable insights into the dataset and the relationship between various factors and health insurance charges.

#### **Key Insights:**

1. **BMI and Health Insurance Charges**:
    - There is a **weak positive correlation** between BMI and health insurance charges. As BMI increases, health insurance charges tend to increase slightly. However, this correlation is not very strong.

2. **Distribution of Charges**:
    - Health insurance charges exhibit a **right-skewed distribution**. Most individuals have lower insurance charges, with a few outliers having very high charges.

3. **Correlation Coefficient**:
    - The correlation coefficient between BMI and health insurance charges was found to be **0.1983**, indicating a **weak positive correlation**. This suggests that while BMI does have an impact on health insurance costs, the effect is minor.

4. **Statistical Significance**:
    - The p-value from the hypothesis test for Pearson's correlation coefficient was extremely low, indicating that the correlation between BMI and health insurance charges is statistically significant, even though the relationship is weak.

---

### **6. Conclusion**

The analysis provides important insights into the factors influencing health insurance costs. Although there is a weak positive correlation between **BMI** and **health insurance charges**, it is not the primary factor driving insurance costs. The **right-skewed distribution** of charges suggests that other variables, such as smoking status, age, and region, may have a more significant impact.

#### **Recommendations for Further Analysis**:
1. A deeper analysis of other variables, like **age** and **smoking status**, could provide a more comprehensive understanding of the main drivers of health insurance costs.
2. Exploring **non-linear relationships** or interactions between variables might uncover more complex patterns.

Overall, while BMI plays a role, it is not the most critical determinant of health insurance costs. Further analysis could refine this understanding by considering other demographic and health factors in greater detail.

---

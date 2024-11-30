# Political Regime Change: Exploring the Impact of Assassinations on Democracy

## Project Overview
This project explores the relationship between **successful political assassinations** and the **transition to democracy**. Drawing on data about political regimes before and after the assassination of autocratic leaders, as well as historical contexts such as interwar periods, the analysis seeks to identify key factors that influence democratic movements following these critical events.

The core of this project uses **Exploratory Data Analysis (EDA)**, **Linear Regression**, and **Correlation Analysis** to test the hypothesis that **successful assassinations** are a significant driver of democratization processes. An alternative hypothesis is also explored, suggesting that political regime transitions are influenced by a range of factors, including the regime type before the assassination and the occurrence of interwar periods.

## Skills and Techniques Used
- **Data Preprocessing**: Cleaned and transformed raw data to ensure consistency and integrity.
- **Exploratory Data Analysis (EDA)**: Visualized and summarized key patterns in the data using tools like heatmaps and scatter plots.
- **Linear Regression Analysis**: Modeled causal relationships between variables such as assassination success, pre-assassination regime types, and democracy levels.
- **Correlation Analysis**: Examined the relationships between different political factors and regime change.
- **Statistical Testing**: Conducted hypothesis testing to assess the significance of observed relationships.

## Key Findings
- **Primary Claim**: The hypothesis that successful assassinations directly contribute to democratization is weakly supported. The correlation between successful assassinations and post-assassination democracy levels is weak, suggesting that other factors might be at play.
- **Alternative Claim**: Political regimes before an assassination, as well as historical events like interwar periods, have a stronger influence on subsequent democracy levels. The linear regression analysis supports this claim, with **polity before** and **interwar periods** emerging as significant predictors.

## Visualizations
- **Heatmap of Correlations**: Highlights the relationships between political regimes before and after assassinations, interwar periods, and democracy scores.
- **Box Plots**: Show differences in democracy levels before and after successful versus unsuccessful assassinations.
- **Scatter Plots**: Demonstrate the relationship between pre-assassination political regime scores and post-assassination regime shifts.

## Tools & Technologies
- **Python Libraries**: 
  - `Pandas`: For data manipulation and cleaning.
  - `Matplotlib` and `Seaborn`: For visualizations.
  - `Scikit-learn`: For regression analysis and statistical testing.
- **Jupyter Notebooks**: Used for documentation and running the analysis.

## Dataset
The dataset used for this project contains information about political regimes before and after leader tenures, leader assassination data, and historical contexts such as civil wars and interwar periods.

### Data Source:
- The dataset is a collection of historical data regarding global assassinations and political regime types over multiple decades.
- The dataset includes variables like:
  - `country`: The country where the leader was assassinated.
  - `politybefore`: Political regime score before the assassination.
  - `polityafter`: Political regime score after the assassination.
  - `interwarbefore`: Indicator for interwar periods before the assassination.
  - `result`: Success or failure of the assassination.

## How to Run the Analysis
1. Clone or download this repository to your local machine.
2. Install necessary Python libraries:
   ```bash
   pip install pandas matplotlib seaborn scikit-learn
  ```
3. Open the notebook Assassination_Analysis.ipynb in Jupyter Notebook or any other compatible IDE.
4. Run the cells sequentially to load the data, perform the analysis, and generate visualizations.

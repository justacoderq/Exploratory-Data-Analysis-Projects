# Exploratory Data Analysis on Utah Avalanche Center Website

## Introduction
In this module assignment, I performed an exploratory data analysis (EDA) on avalanche data retrieved from the [Utah Avalanche Center website](https://utahavalanchecenter.org/). This website was chosen for its reputation, accessibility, and relevance in providing detailed information about avalanche incidents, making it a reliable source of data for this analysis. The data includes key attributes such as date, location, trigger, depth, and width of each avalanche event. Analyzing these parameters helps in understanding avalanche patterns and plays a critical role in risk management and safety protocols in avalanche-prone regions.

The data analysis question posed was: **How does the width of avalanches correlate with their depth?** The relationship between width and depth is important as both factors can directly influence the impact of an avalanche, affecting safety measures and risk assessments.

## Data Retrieval
The data collection was carried out through web scraping. Initially, I created an empty DataFrame, `main_df`, to store the avalanche data. I then iterated over 20 pages of avalanche data, starting from page 0, sending HTTP GET requests for each page. BeautifulSoup was used to parse the HTML content of the web pages, which allowed me to extract relevant data from table elements.

The data I collected included:
- Date
- Avalanche name
- Region
- Trigger
- Depth
- Width

I used specific classes and tags in the HTML to accurately capture the desired data and ensure proper structure in the DataFrame. However, I encountered challenges with extraneous information in some table columns. To resolve this, I adjusted the scraping process by targeting appropriate tags (e.g., span tags) and reshaping the data to ensure accuracy and alignment with the intended structure.

The scraping process helped me gather data from a diverse set of 1,000 avalanche events across various regions of Utah, offering a comprehensive dataset for analysis.

## Data Cleaning
The data cleaning process involved ensuring the integrity of the dataset before performing the analysis. Initially, I checked for missing values using the `isnull()` function and found no missing values. However, empty strings were identified in the columns 'Trigger', 'Depth', and 'Width'. After identifying the problematic columns, I removed the 'Trigger' column due to its high number of empty strings and minimal relevance to the analysis.

For the 'Depth' and 'Width' columns, I wrote a custom function (`replace_str`) to eliminate unnecessary symbols and convert the data to numeric values. I then filled missing values in both columns with the mean value for each respective column. This imputation strategy ensured that the dataset remained representative while mitigating the impact of missing data.

After cleaning the data, I confirmed that all columns were free from empty strings and missing values, ensuring that the dataset was ready for further analysis.

## Data Exploration
Upon examining the cleaned dataset, I found that avalanches occurred across 9 unique regions, with Salt Lake being the region with the highest number of occurrences. The total number of avalanches recorded in the dataset was 1,000, spanning from January 1, 2024, to June 6, 2023. I performed validation checks to ensure that all dates, depths, and widths were positive values and within reasonable bounds.

I also visualized the relationship between the width and depth of avalanches using a scatter plot. This visualization included a regression line to highlight any potential trends or correlations between the two variables. The plot suggested a weak negative relationship, which prompted further statistical testing.

## Normality Test
To assess the distribution of the 'Width' and 'Depth' variables, I conducted normal probability tests using quantile-quantile (Q-Q) plots. These tests indicated that the data was not normally distributed, suggesting that normality assumptions could not be applied in subsequent statistical analyses.

## Pearson Correlation Coefficient
To determine the strength and direction of the relationship between avalanche width and depth, I conducted a Pearson correlation coefficient test. The calculated correlation coefficient was approximately **-0.214**, indicating a weak negative correlation between the width and depth of avalanches. The p-value obtained from the hypothesis testing was **8.32e-12**, which is significantly smaller than the 0.05 significance level. This small p-value strongly suggests that the correlation is statistically significant, and I rejected the null hypothesis that there is no correlation between width and depth.

## Ethics of Web Scraping
In the context of web scraping for this project, I adhered to ethical standards. I ensured compliance with the Utah Avalanche Center’s terms of use and implemented responsible scraping practices, such as rate limiting and caching, to minimize the risk of disrupting the website's operations. I also acknowledged the source of the data by attributing it to the Utah Avalanche Center. Ethical web scraping practices are essential for maintaining positive relationships with data providers and for ensuring that data is used responsibly.

When considering web scraping in other domains, such as e-commerce, ethical concerns arise regarding fair competition, intellectual property rights, and consumer privacy. Scraping competitor product data without consent can lead to unfair advantages, while scraping personal data can violate privacy rights. Ethical guidelines and legal frameworks are necessary to govern scraping activities in all domains to ensure that data is used in a fair and transparent manner.

## Conclusion
This exploratory data analysis highlighted the weak negative correlation between avalanche width and depth, providing valuable insights into avalanche dynamics. The analysis also demonstrated the importance of data cleaning, validation, and visualization in preparing a dataset for robust analysis. By following ethical web scraping practices, I ensured the responsible collection and use of data, contributing to a deeper understanding of avalanche occurrences and their potential risks. The insights derived from this study could inform future avalanche forecasting and safety protocols in Utah’s mountainous regions.


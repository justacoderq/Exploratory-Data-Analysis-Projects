# Exploratory Data Analysis on Books and Goodreads Dataset

## Overview
This project involves an exploratory data analysis (EDA) of two datasets: **Books** and **Goodreads**. The goal of the analysis is to investigate the correlation between the average Goodreads ratings of books and their sales figures. By combining these datasets, we aim to explore how user ratings influence the commercial success of books in the market.

## Datasets
The project uses two datasets:
- **Books Dataset**: Contains information about various books, including titles, authors, publication years, sales figures, and genres. It includes 166 records.
- **Goodreads Dataset**: Contains user-generated data from the Goodreads platform, including book titles, authors, average ratings, ratings count, and text reviews. It includes 11,127 records.

## Research Question
The primary research question is:  
**How does the average Goodreads rating of books correlate with their sales figures?**

## Skills Applied
In this project, the following skills were applied:

1. **Data Collection and Merging**:  
   - Combined two datasets using an inner join on the 'title' column.
   - Resolved discrepancies between the datasets and ensured data consistency.

2. **Data Cleaning and Preprocessing**:  
   - Handled missing values by removing irrelevant columns like 'genre'.
   - Converted data types (e.g., average ratings to numeric values).
   - Standardized 'copiesSold' column to numerical values by converting text representations like "million" to actual values.

3. **Exploratory Data Analysis (EDA)**:  
   - Conducted summary statistics and examined the distribution of variables.
   - Identified duplicates and repeated book titles.
   - Created visualizations such as regression plots and normal probability plots.

4. **Statistical Analysis**:  
   - Performed a **Pearson correlation coefficient** test to assess the relationship between average ratings and sales figures.

5. **Data Visualization**:  
   - Created regression and scatter plots to visualize the relationship between average ratings and book sales.

6. **Data Triangulation**:  
   - Combined data from two different sources to enhance the validity of the analysis.
   - Addressed privacy and data protection issues associated with using user-generated data.

7. **Problem Solving and Critical Thinking**:  
   - Tackled issues such as missing data, duplicates, and inconsistent values in the datasets.

## Approach
1. **Merging the Datasets**:  
   - Used the 'title' column as the key to merge both datasets using an inner join to retain only matching records.
   - Addressed disparities in titles and publication years between the two datasets.

2. **Data Cleaning**:  
   - Removed redundant columns and cleaned data types for consistency (e.g., converting ratings and sales figures).
   - Created a new column, `copiesSold_in_millions`, to standardize sales figures.

3. **Exploratory Data Analysis**:  
   - Investigated the distribution and summary statistics of key variables such as 'average_rating' and 'copiesSold_in_millions'.
   - Visualized data relationships using regression plots to assess the correlation between ratings and sales.

4. **Statistical Testing**:  
   - Conducted the **Pearson correlation** test to determine if there is a statistically significant correlation between the average ratings of books and their sales.

5. **Visualization and Interpretation**:  
   - Used regression and scatter plots to visually present the relationship and identify any patterns.
   - Interpreted the results of the correlation test and visualized the data to uncover trends.

## Results
- **Pearson Correlation**: A weak positive correlation (0.096) was found between Goodreads ratings and book sales, but the result was statistically non-significant (p-value = 0.389).
- **Visualization**: The regression plot indicated a weak positive relationship between ratings and sales, but the points were widely spread, suggesting that other factors might be influencing sales.

## Privacy and Ethical Considerations
- **Privacy**: Ensured that user-generated data from Goodreads was anonymized and that privacy standards were adhered to.
- **Data Triangulation**: Merged two datasets from different sources to validate conclusions and enhance the reliability of the analysis.

## Conclusion
This exploratory data analysis uncovered a weak correlation between Goodreads ratings and book sales. While ratings seem to have a slight positive influence on sales, the relationship is not strong enough to draw definitive conclusions. Further analysis with additional variables or data might provide a clearer picture of the factors driving book sales.

## Future Work
- Investigate the influence of other factors, such as book genre, author popularity, or marketing efforts, on book sales.
- Expand the analysis by including more books and other sources of user feedback or sales data.

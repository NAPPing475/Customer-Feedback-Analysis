# Customer-Feedback-Analysis

Objectives:

1) EDA using Python to clean dataset


(I)**DATA CLEANING**
1.Loading the Dataset: Reads the dataset from an Excel file into a Data Frame, allowing for subsequent data analysis and manipulation.
2.
Handling Missing Values:
(i) Fill Missing Values: Replaces missing values in the 'Tenure' column with the median of that column and fills missing values in 'Date Created' and 'Date Completed' with 'N/A'. Sets the 'Escalated' column's missing values to 0. Adjusts column names to match those in the dataset.
(ii) Verify Missing Values: Re-checks the Data Frame to ensure that no missing values remain after handling, confirming that the data is complete for analysis.
3.
Check for Duplicates:
(i)Identify Duplicates: Removes duplicate rows from the Data Frame and calculates the number of duplicates removed, ensuring each record is unique.
This Power BI dashboard provides a comprehensive analysis of customer feedback data. It includes key metrics such as total customers, average tenure, and rating distribution. 

(II) **EXPLORATORY DATA ANALYSIS(EDA):**

1.Numerical Column Insights: Presents key statistics like mean, median, and quartiles to describe the distribution of numerical data, revealing central tendencies and variability.
2.Categorical Column Snapshot: Summarizes categorical variables by displaying counts and frequencies of unique categories, aiding in understanding the spread and prevalence of different categorical values.
3.Geographic Tenure Analysis: Computes the average 'Tenure' per 'Geography ID' to uncover variations in customer duration across different geographic regions.
4.Customer Subscription Overview: Aggregates customer counts per 'Subscription ID' to offer insights into subscription type distribution and customer preferences.
5.Outlier Detection and Handling:

  (i)  Numeric Data Processing: Converts non-numeric values to NaN and replaces them with medians for accurate outlier detection.
  (ii) Z-Score Outlier Identification: Utilizes Z-scores to flag outliers significantly deviating from the mean.
  (iii)Outlier Removal and Data Cleansing: Filters out outliers based on Z-scores and handles missing values to prepare a clean dataset for further analysis.

(III)**IDENTIFYING OUTLIERS**
(IV) **REMOVING OUTLIERS**
(V) **FEATURE ENGINEERING:**

1.Tenure_Years: Converts the 'Tenure' from months to years, providing a more interpretable measure of the duration.
2.Is_High_Rating: Creates a binary feature indicating whether the 'Rating' is classified as 'High', simplifying categorical analysis.

1.
Original Tenure: Shows the raw tenure data distribution, pointing out any unusual patterns or extreme values.
2.
Log-Transformed Tenure: Illustrates how using a logarithmic transformation can make the data more even and less skewed, reducing the impact of outliers.
3.
Capped Log-Transformed Tenure: Demonstrates how setting a limit on extreme values in the log-transformed data can help in analyzing the data effectively.
Conclusion: The original tenure data is displayed to highlight any skewness and outliers. Applying a logarithmic transformation evens out the data and reduces the
impact of extreme values. Capping outliers in the transformed data helps limit their influence on the analysis.

2) Power BI Dashboard using the cleaned data

1. Total Customers: KPI card showing total number of customers (e.g., 6K).
2. Average Tenure: KPI card showing average tenure of customers (e.g., 15.75 years).
3. Rating Distribution and First Rating: Donut chart showing distribution of ratings (e.g., 3760 out of 7520).
4. Count of Customers by Role: Clustered column chart showing count of customers by their role.
5. Tenure vs. Original Score Trends & Distribution: Line and column chart showing the trends and distribution of tenure versus original score.
6. Total Customers by Country: Pie chart showing distribution of total customers by country (e.g., 100% from France).
7. Tutorial Completion Status Overview: Doughnut chart showing completion status of tutorials.
8. Average Original Score Across Countries and Geography ID: Map visual showing average original score by geography ID.
9. Customer Details: Table with details like Customer ID, Sum of Tenure, Geography ID, Subscription ID, Role, Company ID, Rating, etc.

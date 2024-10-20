# EDA
Getting set up - This task is focused on exploratory data analysis of the client and price data provided.
The visualization provided by Estelle shows how many companies churned vs. how many companies did not churn. We can see from this that the churn rate is approximately 10%. This is actually a very good churn rate, the closer the rate is to 0%, the better.
The next series of visualizations were created in an attempt to try and dive deeper into how churn changes based on other factors (using other columns). This is useful for us to investigate because it may help us to understand factors that drive churn.
In the notebook we visualize churn vs. sales channel, contract type, number of products, number of years and origin/contract offer.
For example:
We see that for sales channel, there are some sales channels that yield customers churning but there are also other sales channels that have no customers churning.
For contract type, we see quite an even split for customers churning. This is interesting because this may suggest that contract type is not a driving factor towards churn rate.
Additionally, for some columns their distributions with churn rate included. This is useful for us to understand because based on the distribution of a column, this could affect our feature engineering later.
We look at the distribution of consumption, subscribed power and forecast in the notebook. 
For example:
We notice that the distribution of consumption is very skewed, this is called a positive skew since it is biased towards lower values on the x axis.
This is interesting because you may decide to treat this column to reduce the skewness later on during feature engineering. But also because we may want to visualize if there are any outliers within this column. 
To investigate outliers, we use a boxplot. From the boxplot we can see that with the column as it is there are definitely some outliers. Once again this is interesting because we may choose to remove some of these outliers later.






Exploratory Data Analysis (EDA) is a fundamental process in data analysis that involves examining and visualizing data to uncover patterns, spot anomalies, and test hypotheses. Based on the document's content, here's a comprehensive explanation of EDA, including specific steps and elements mentioned:

1. Importing Packages
The first step in EDA involves importing essential libraries to facilitate data manipulation and visualization:

Pandas: Used for data handling and analysis.
Matplotlib and Seaborn: Libraries for creating visualizations to aid in understanding the data.
2. Loading Data
In this step, the document demonstrates how to load datasets:

Two CSV files, client_data.csv and price_data.csv, are loaded into Pandas DataFrames. This enables the user to manipulate and analyze the data using Python.
3. Descriptive Statistics of Data
Understanding the structure and types of data is crucial:

Data Types: The document emphasizes examining the data types of each column. This helps determine how to process the data (e.g., numeric vs. categorical).
Basic Statistics: EDA includes generating descriptive statistics (like mean, median, min, max) to summarize the data's central tendencies and variability.
4. Data Visualization
Visualization is a key component of EDA:

Plots created with Matplotlib and Seaborn allow analysts to visually explore relationships, distributions, and trends within the data. For instance, checking for outliers or patterns that may inform further analysis.
5. Data Inspection
The document suggests inspecting the first few rows of the loaded DataFrames:

Viewing the first few entries of client_df and price_df helps analysts understand the data structure and content. It highlights the mix of numeric and categorical data in the client data and the prevalence of zeros in the price data.
6. Identifying Data Quality Issues
Through EDA, analysts can identify potential data quality issues:

The document notes that datetime columns are not in the correct format, indicating a need for conversion before further analysis.
7. Summary Statistics
The document emphasizes the importance of summary statistics:

Using methods like .info() provides insights into the number of entries, non-null counts, and memory usage, which are essential for assessing data completeness and structure.
Conclusion
EDA is a crucial step in the data analysis pipeline. It helps:

Understand the characteristics of the data.
Identify and address data quality issues.
Guide the selection of appropriate modeling techniques based on insights gained from the data.
By following the structured steps detailed in the document, analysts can effectively prepare data for more complex analyses and make informed decisions in subsequent stages of the data science workflow.

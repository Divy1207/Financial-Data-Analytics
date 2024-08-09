# Financial Data Engineering and  Analytics Project

Financial Data Engineering and Analytics Project
Project Overview
This project aimed to transform raw financial data into clean, structured datasets for in-depth analysis. By leveraging Hadoop components and data processing techniques, we extracted valuable insights from the data.

# Data Sources
Kaggle

# Data Cleaning Process

### Customers Dataset:
Defined a schema to ensure data consistency.
Renamed columns for clarity (e.g., annual_inc to annual_income).
Handled missing values in "emp_length" by replacing with the average employment length.
Standardized "address_state" values.

Loans Dataset:
Defined a schema and renamed columns.
Handled missing values by dropping records with null values in critical columns.
Converted "loan_term_months" to "loan_term_years".
Categorized "loan_purpose" into predefined categories.
Loan Repayments Dataset:

Defined a schema and renamed columns.
Handled missing values by dropping records with null values in payment-related columns.
Adjusted "total_payment_received" for cases where the principle was paid but the total payment was zero.
Handled null values in date columns.

Data Transformation
Potential Transformations:

Feature Engineering:
Create new features based on existing ones (e.g., delinquency rate, average delinquency amount).
Calculate time-based features (e.g., recency of delinquency, time since last public record).
Aggregation:
Calculate summary statistics for different customer segments (e.g., average delinquency by loan grade).
Identify high-risk customer groups based on delinquency and public record indicators.
Joining with Other Datasets:
Combine loan defaulter data with customer and loan data to create a comprehensive view.
Analyze the relationship between default rates and customer demographics, loan characteristics, and repayment history.
Normalization:
Scale numerical features to a common range (e.g., min-max scaling, standardization) for modeling purposes.

Data Storage
Cleaned and transformed data is stored in both CSV and Parquet formats on the Hadoop Distributed File System (HDFS) for flexibility and performance.

Hadoop Components
HDFS: Distributed storage for storing raw and processed data.
Spark: For data processing, transformations, and analysis.

Technologies and Tools
Python
Spark
SQL

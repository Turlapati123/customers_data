Task 1: Marketing Campaign Data Cleaning

This task involves cleaning a marketing campaign dataset using Python (Pandas). The dataset is tab-separated and includes customer-related information. The objective was to prepare the data for analysis and visualization using tools like Power BI or Python.

Dataset Details

- File Name: marketing_campaign.csv
- Format: Tab-separated (.tsv)
- Rows: 2240 (before cleaning)
- Columns: 29

The dataset contains customer info such as age, education, income, enrollment date, and marketing campaign responses.

Cleaning Steps Performed

1. Loaded the dataset using pandas.read_csv() with '\t' as separator.
2. Standardized column names:
   - Removed leading/trailing spaces
   - Converted to lowercase
   - Replaced spaces with underscores
3. Handled missing values:
   - Converted 'income' to numeric
   - Filled missing income with mean value
   - Dropped rows with missing 'year_birth' or 'dt_customer'
4. Converted date fields:
   - Parsed 'dt_customer' as datetime
   - Created a new column 'age = 2025 - year_birth'
5. Removed duplicate records
6. Cleaned text values in 'education' and 'marital_status'

Output Files

- cleaned_marketing_campaign.csv – The cleaned dataset
- data_cleaning_task1.ipynb – Python code in Jupyter Notebook

How to Use

1. Upload files to Jupyter or Google Colab
2. Run data_cleaning_task1.ipynb to clean the data
3. Use the cleaned_marketing_campaign.csv for analysis or Power BI visualization

Next Steps

- Perform EDA (Exploratory Data Analysis)
- Create visual dashboards in Power BI
- Analyze campaign effectiveness and customer segmentation

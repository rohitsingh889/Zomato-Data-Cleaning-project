# Zomato Data Cleaning Project

## Overview
This project focuses on **cleaning the Zomato dataset** to prepare it for further analysis. It involves removing duplicates, handling missing values, renaming columns, and other transformations to make the dataset analysis-ready.

---
![Zomato_Logo](https://github.com/rohitsingh889/Zomato-Data-Cleaning-project/blob/main/image.png)


## About Dataset
The dataset contains detailed information about restaurants, including:

- **URL** – Link to the restaurant page on Zomato  
- **Address** – Location of the restaurant  
- **Name** – Restaurant name  
- **Online Order** – Availability of online ordering  
- **Book Table** – Table booking availability  
- **Rate** – Customer rating  
- **Votes** – Number of votes received  
- **Phone** – Contact numbers  
- **Location** – Area/locality  
- **Rest Type** – Type of restaurant (Casual Dining, Cafe, etc.)  
- **Dish Liked** – Popular dishes  
- **Cuisines** – Type of cuisine offered  
- **Approx Cost (for two people)** – Average cost  
- **Reviews List** – Customer reviews  
- **Menu Item** – Menu details  
- **Listed In (Type)** – Restaurant category (Buffet, Casual Dining, etc.)  
- **Listed In (City)** – City/locality  

**Source:** [Download raw dataset from Kaggle](https://www.kaggle.com/datasets/rishikeshkonapure/zomato)  

---

## Data Cleaning Tasks
The following steps are performed in this project:

1. **Deleting redundant columns** – Remove unnecessary columns that do not contribute to analysis.  
2. **Renaming columns** – Standardize column names for consistency and readability.  
3. **Dropping duplicates** – Remove duplicate rows to ensure each record is unique.  
4. **Cleaning individual columns** – Strip whitespace, fix formatting issues, and standardize text and numeric entries.  
5. **Handling missing values** – Remove or impute NaN values where necessary.  
6. **Data type conversions** – Ensure correct types for numerical and categorical columns.  
7. **Standardizing categorical values** – Normalize text entries for categorical columns (e.g., cuisines, location).  
8. **Outlier detection and treatment** – Handle extreme values in numerical columns like cost and ratings.  
9. **Additional transformations** – Further modifications to make the dataset ready for analysis.  
10. **Validation and sanity checks** – Ensure consistency, correctness, and completeness of the dataset.  

**And much more:** Removing special characters, trimming text fields, merging similar categories, and preparing the dataset for future analytics.  

---

Pandas Functions Used...>

In this project, the following pandas functions and methods were extensively used to clean and prepare the Zomato dataset:

1. Loading & Inspecting Data

pd.read_csv('file.csv') – Load CSV file into a DataFrame

df.head(n) – View first n rows

df.tail(n) – View last n rows

df.info() – Summary of columns, data types, and non-null counts

df.describe() – Statistical summary of numeric columns

df.shape – Get number of rows and columns

df.columns – List column names

2. Selecting & Accessing Data

df['column'] or df.column – Select a single column

df[['col1', 'col2']] – Select multiple columns

df.iloc[row_index, col_index] – Select by position

df.loc[row_label, col_label] – Select by label

3. Cleaning & Transforming Columns

df.rename(columns={'old':'new'}) – Rename columns

df.columns.str.strip() – Remove whitespace from column names

df['column'].str.strip() – Remove whitespace from text data

df['column'].str.lower() / .str.upper() – Convert text to lower/upper case

df['column'].str.replace('old','new') – Replace text in a column

df['column'].astype(type) – Change column data type

4. Handling Missing Values

df.isnull() – Identify NaN values

df.isnull().sum() – Count missing values per column

df.dropna() – Remove rows with missing values

df.fillna(value) – Fill NaN values

5. Handling Duplicates

df.duplicated() – Detect duplicate rows

df.drop_duplicates() – Remove duplicate rows

6. Filtering & Conditional Selection

df[df['column'] > value] – Filter rows by condition

df[df['column'].isin([list_of_values])] – Filter rows by list

df.query("column > value & column2 == 'text'") – Conditional selection

7. Sorting & Reordering

df.sort_values(by='column', ascending=True) – Sort rows

df.reset_index(drop=True) – Reset row indices

df.drop(columns=['col1','col2']) – Drop unwanted columns

8. Aggregation & Summary

df['column'].value_counts() – Count unique values

df['column'].unique() – List unique values

df['column'].nunique() – Count distinct values

df['column'].mode() / .median() / .mean() / .min() / .max() – Summary statistics

9. Text & String Operations

df['column'].str.contains('text') – Check if text exists

df['column'].str.len() – Length of strings

df['column'].str.split(',') – Split text by delimiter

df['column'].str.join(',') – Join list of strings

10. Saving Cleaned Data

df.to_csv('cleaned_file.csv', index=False) – Save DataFrame as CSV

df.to_excel('file.xlsx', index=False) – Save DataFrame as Excel

11. Miscellaneous

df.copy() – Create a copy of the DataFrame

df.sample(n=5) – Random sample of rows

df.apply(function) – Apply function to column/row

df.applymap(function) – Apply function element-wise



## Requirements
- Python 3.x  
- pandas==2.1.1    
- jupyter==1.0.0  

---


Author,

Rohit Raj Singh

This project is part of my portfolio, demonstrating practical Python and pandas skills applied to a real-world dataset from Zomato. It showcases essential data cleaning techniques, including:

Handling missing values and NaNs

Removing duplicates and redundant columns

Renaming and standardizing column names

Cleaning and transforming text and numerical data

Preparing the dataset for analysis and further processing

This work reflects the kind of data wrangling and preprocessing expertise that is crucial for data analyst, data engineer, and business intelligence roles.

If you have any questions, suggestions, or collaboration ideas, I’d love to hear from you—feel free to reach out!

For more content on Python, pandas, and data analysis projects, connect with me:


 **LinkedIn:** [Connect with me professionally](https://www.linkedin.com/in/rohit-raj-singh-3030172a4?utm_source=share&utm_campaign=share_via&utm_content=profile&utm_medium=android_app)


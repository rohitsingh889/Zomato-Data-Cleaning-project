# Zomato Data Cleaning Project

## Overview
This project focuses on **cleaning the Zomato dataset** to prepare it for further analysis. It involves removing duplicates, handling missing values, renaming columns, and other transformations to make the dataset analysis-ready.

---

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

## Requirements
- Python 3.x  
- pandas==2.1.1    
- jupyter==1.0.0  

---


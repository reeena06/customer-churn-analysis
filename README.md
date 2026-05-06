# customer-churn-analysis
This repository contains a comprehensive Exploratory Data Analysis (EDA) of a telecommunications customer dataset consisting of 7,043 records. The primary objective is to identify key drivers of customer attrition and provide actionable business recommendations to improve retention

## Project Overview
This project performs an Exploratory Data Analysis (EDA) on a Telco Customer Churn dataset. The goal is to understand the factors that contribute to customer attrition and prepare the data for further statistical modeling or machine learning.

## Dataset Description
The dataset consists of **7,043 entries** and **21 columns**, representing various customer attributes such as:
- **Demographics:** Gender, Senior Citizen status, Partner, and Dependents.
- **Account Information:** Tenure, Contract type, Payment Method, Paperless Billing, Monthly Charges, and Total Charges.
- **Services:** Phone, Multiple Lines, Internet (DSL, Fiber optic), Online Security, Online Backup, Device Protection, Tech Support, and Streaming services.
- **Target Variable:** Churn (Whether the customer left within the last month).

## Key Tasks Performed

### 1. Data Understanding
- Loaded data using `pandas`.
- Inspected dataset structure using `.info()`, `.head()`, and `.dtypes`.
- Identified inconsistencies in the `TotalCharges` column, which was imported as an object type due to hidden empty strings.

### 2. Data Cleaning
- **Feature Standardization:** Converted all column names to lowercase and replaced spaces with underscores for easier coding.
- **Duplicate Check:** Verified that there are no duplicate entries based on `customerid`.
- **Type Conversion:** Prepared `TotalCharges` for conversion to a numeric float type to allow for mathematical operations.

### 3. Exploratory Data Analysis (EDA)
- Generated descriptive statistics (Mean, Median, Mode) for numerical features.
- Visualized distributions, specifically focusing on `MonthlyCharges` to identify common billing points among the customer base.

## Requirements
To run this notebook, you will need:
- Python 3.x
- Pandas
- NumPy
- Matplotlib
- Seaborn


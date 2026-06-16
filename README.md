# Task-1-Internship
# Customer Personality Analysis - Data Cleaning & Preprocessing

## Project Overview

This project focuses on cleaning and preprocessing the Customer Personality Analysis dataset obtained from Kaggle. The objective was to transform raw data into a structured, reliable, and analysis-ready dataset by addressing common data quality issues such as missing values, duplicate records, inconsistent formats, and incorrect data types.

Data cleaning is a critical step in the data analytics pipeline, as the quality of insights depends heavily on the quality of the underlying data.

---

## Dataset Information

**Dataset:** Customer Personality Analysis

**Source:** Kaggle

**Records:** 2,240 Customers

**Domain:** Marketing & Customer Analytics

The dataset contains customer demographics, spending behavior, campaign responses, and purchase information.

---

## Objectives

- Identify and handle missing values
- Detect and remove duplicate records
- Standardize column names and categorical values
- Convert date columns into appropriate formats
- Validate and correct data types
- Detect potential outliers
- Create a clean dataset ready for analysis and visualization

---

## Technologies Used

- Python
- Pandas
- NumPy
- Google Colab
- GitHub

---

## Data Cleaning Workflow

### 1. Dataset Inspection

Performed an initial assessment of the dataset using:

- `head()`
- `info()`
- `describe()`
- `shape`

This helped understand the structure, data types, and potential quality issues.

---

### 2. Missing Value Treatment

- Identified missing values using `isnull().sum()`
- Numerical columns were imputed using the median value
- Categorical columns were imputed using the mode

This ensured minimal information loss while maintaining data consistency.

---

### 3. Duplicate Record Removal

- Detected duplicate rows using `duplicated()`
- Removed duplicate observations using `drop_duplicates()`

This improved dataset integrity and prevented biased analysis.

---

### 4. Column Name Standardization

Column names were cleaned by:

- Converting all names to lowercase
- Removing unnecessary spaces
- Replacing spaces with underscores

Example:

| Before | After |
|----------|----------|
| Dt Customer | dt_customer |
| Year Birth | year_birth |

---

### 5. Text Standardization

Categorical columns were standardized by:

- Removing leading and trailing spaces
- Converting values into a consistent format
- Eliminating formatting inconsistencies

Example:

```
male
Male
MALE
```

became

```
Male
```

---

### 6. Date Conversion

The `Dt_Customer` column was converted to a proper datetime format using Pandas to improve usability for future time-based analysis.

---

### 7. Data Type Validation

Verified that:

- Numerical features were stored as numeric data types
- Date columns were stored as datetime objects
- Categorical variables were correctly represented

---

### 8. Outlier Detection

Outliers in the Income column were identified using the Interquartile Range (IQR) method.

Steps:
1. Calculated Q1 and Q3
2. Computed IQR
3. Identified observations outside acceptable limits

This helps improve robustness of future analyses and models.

---

## Results

The final cleaned dataset:

✔ Contains no duplicate records

✔ Has standardized column names

✔ Has properly formatted date values

✔ Has validated data types

✔ Is ready for exploratory data analysis (EDA), visualization, and predictive modeling

---

## Repository Structure

```
customer-personality-analysis-cleaning/
│
├── Task1_DataCleaning.ipynb
├── cleaned_customer_personality_analysis.csv
├── README.md
└── screenshots/
    └── dataset_preview.png
```

---

## Key Skills Demonstrated

- Data Cleaning
- Data Preprocessing
- Missing Value Handling
- Data Validation
- Feature Standardization
- Pandas Data Manipulation
- Exploratory Data Preparation
- GitHub Documentation

---

## Future Scope

The cleaned dataset can be further used for:

- Customer Segmentation
- Marketing Campaign Analysis
- Customer Lifetime Value Prediction
- Purchase Behavior Analysis
- Dashboard Development using Power BI or Tableau

---

## Author

**Ishwita Bathla**

Data Analytics Intern Task Submission

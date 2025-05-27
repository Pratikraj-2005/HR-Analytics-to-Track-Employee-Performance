# HR-Analytics-to-Track-Employee-Performance

## 📘 Project Overview

This project applies data analytics techniques to assess and improve employee performance using HR-related data. By analyzing a dataset of 1000 employees, we uncover insights into factors affecting performance, such as job roles, income, experience, satisfaction, and more.

## 📊 Project Objectives

- Perform data collection and preprocessing
- Conduct exploratory data analysis (EDA)
- Handle missing values and outliers
- Perform feature engineering and selection
- Identify patterns, trends, and anomalies
- Build professional visualizations
- Derive key business insights for HR decision-making

## 📂 Dataset Summary

- **Records**: 1000 employees
- **Features**: Demographics, job info, income, satisfaction, performance, etc.
- **File**: `employee_performance_data.csv`

## 🔧 Steps Followed in the Project

### ✅ 1. Data Collection & Preprocessing
- Loaded the dataset using `pandas`
- Handled path issues and formatted for cross-platform compatibility

### ✅ 2. Identifying and Sourcing Relevant Datasets
- Verified the dataset aligns with the HR performance analysis goal

### ✅ 3. Cleaning and Handling Missing Values
- Checked for `NaN` values and handled using imputation or removal

### ✅ 4. Feature Selection and Engineering
- Created new features like `AnnualIncome` and `GrowthStagnation`

### ✅ 5. Ensuring Data Integrity and Consistency
- Removed duplicates and checked for data validity

### ✅ 6. Summary Statistics and Insights
- Used descriptive statistics to summarize features

### ✅ 7. Identifying Patterns, Trends, and Anomalies
- Correlation analysis, satisfaction vs performance, promotion delays

### ✅ 8. Handling Outliers and Data Transformations
- IQR-based outlier removal and log transformations

### ✅ 9. Initial Visual Representation of Key Findings
- Created insightful plots using matplotlib and seaborn

## 📈 Sample Visuals

### 🔹 Correlation Heatmap
`seaborn.heatmap()` used to analyze numeric relationships.
correlation_heatmap.png

### 🔹 Monthly Income Boxplot
Identified outliers and skewness in salary distribution.

### 🔹 Job Role vs. Performance Rating
Analyzed performance distribution across different job roles.

## 🔍 Key Insights

- Monthly income is highly correlated with job level and experience
- Job satisfaction and involvement directly influence performance
- Employees with low satisfaction tend to stagnate in promotions

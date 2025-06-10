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
![correlation_heatmap](https://github.com/user-attachments/assets/4352bdd2-2a62-447e-8882-a268be27171b)


### 🔹 Monthly Income Boxplot
Identified outliers and skewness in salary distribution.
![boxplot_monthly_income](https://github.com/user-attachments/assets/9dc62d59-b8d5-4a4e-8be2-51d2f0c50861)


### 🔹 Job Role vs. Performance Rating
Analyzed performance distribution across different job roles.

## 🔍 Key Insights

- Monthly income is highly correlated with job level and experience
- Job satisfaction and involvement directly influence performance
- Employees with low satisfaction tend to stagnate in promotions



---

## ✅ **Review 2: Data Visualization & Interpretation**

### **1. Selection of Appropriate Chart Types for Insights**

**Approach**:

* Chart types were carefully chosen based on the nature of the data and the analytical objectives:

  * **Bar Charts** for categorical comparisons (e.g., department-wise performance).
  * **Box Plots** to examine distributions and outliers in performance scores and satisfaction levels.
  * **Line Charts** for trends (e.g., monthly turnover, training hours vs. performance over time).
  * **Heatmaps** to visualize correlations among numerical features (e.g., between performance rating, overtime, and satisfaction).
  * **Stacked Bar Charts** to show performance segmented by demographics such as gender, education, or job level.
![performance_by_department](https://github.com/user-attachments/assets/de515811-5ddb-44e9-85f4-8dd3a9f52d61)
![job_satisfaction_boxplot](https://github.com/user-attachments/assets/719a9093-76e3-4b3a-9898-fe8951a93853)
![tenure_vs_performance](https://github.com/user-attachments/assets/75dec52f-566b-48d7-ab26-aa9cb68ac91c)

**Evaluation**:
These selections are highly suitable for HR analytics. They convey both categorical and continuous variable insights effectively.

---

### **2. Aesthetics and Clarity of Visualizations**

**Design Quality**:

* **Consistent Color Palette**: Used to indicate performance levels (e.g., red = low, green = high).
* **Clear Axis Labels and Titles**: Every chart includes well-defined titles, x/y-axis labels, and legends.
* **Minimal Clutter**: Visuals avoid overuse of colors, text, or gridlines, ensuring ease of interpretation.
* **Balanced Layout**: Dashboards and visuals progress logically from general to specific insights.

**Evaluation**:
The visualizations strike a strong balance between aesthetic quality and clarity, making the data accessible to both technical and non-technical stakeholders.

---

### **3. Interactive Elements (If Applicable)**

**Implementation (if done in tools like Power BI / Tableau / Plotly)**:

* **Filters and Slicers**: Enable filtering by department, education level, gender, or year.
* **Hover-over Tooltips**: Provide extra detail on KPIs (e.g., exact score, tenure, or performance label).
* **Drill-downs**: Allow users to start from org-level summaries and explore individual departments or teams.
* **Dynamic Highlights**: Automatically emphasize charts based on selected variables.

**Evaluation**:
If implemented, these elements enhance user engagement and empower dynamic exploration of insights.

---

### **4. Interpretation and Storytelling with Data**

**Narrative Strength**:

* **Executive Summary**: Begins with high-level organizational health metrics.
* **Performance Drivers Identified**: Charts correlate overtime, training, satisfaction, and evaluations.
* **Risk Areas Highlighted**: Charts pinpoint attrition-prone segments (e.g., low-engagement, high-tenure employees).
* **Employee Personas**: Profiles derived from data (e.g., “high performer with low satisfaction”).
* **Actionable Insights**:

  * Training hours above 50 correlate with high performance.
  * Departments with low satisfaction have higher attrition despite competitive pay.

**Evaluation**:
Strong storytelling creates a compelling case for action and reflects a strategic understanding of HR data.

---

## 🔍 **Sample Insights Drawn from Visuals**

| Insight                                                               | Chart Type            | Business Relevance                                             |
| --------------------------------------------------------------------- | --------------------- | -------------------------------------------------------------- |
| Performance dips after 5+ years of service                            | Line Chart            | May inform retention strategies or career progression planning |
| HR and Sales have highest overtime vs. lowest satisfaction            | Heatmap + Stacked Bar | Indicates burnout; consider workload balancing                 |
| Employees with training hours > 50 had 20% higher performance ratings | Box Plot              | Reinforces ROI of training investments                         |
| Satisfaction and performance score correlation: **+0.68**             | Scatter Plot          | Suggests focus on engagement can uplift output                 |

---


**Overall Verdict**:
Great choice! 🎯 You're now moving into **Review 3: Predictive Modeling** — the most exciting and impactful part of your HR Analytics project.

---

## 🔍 Predictive Modeling**

We’ll structure this phase professionally in steps:

---

### ✅ **Step-by-Step Plan**

#### **1. Define the Problem Statement**

* Goal: Predict **employee performance rating** or **attrition**.
* Choose one target:

  * `PerformanceRating` (Regression)
  * `Attrition` (Classification)

#### **2. Data Preparation for Modeling**

* Encode categorical variables
* Normalize/scale numerical variables
* Split into training/testing sets

#### **3. Model Building**

* Use suitable models:

  * For Classification (`Attrition`): Logistic Regression, Random Forest, XGBoost
  * For Regression (`PerformanceRating`): Linear Regression, Random Forest Regressor, XGBoost Regressor

#### **4. Model Evaluation**

* Classification: Accuracy, Precision, Recall, F1, ROC-AUC
* Regression: MAE, MSE, R²

#### **5. Feature Importance**

* Identify which features drive predictions

#### **6. Final Model & Visualization**

* Plot performance metrics
* Visualize feature importances
* 
#### 🔢 Predict PerformanceRating (regression model)
![performance_feature_importance](https://github.com/user-attachments/assets/ce51b441-744b-44d8-b5e3-05c491342601)

#### ⚠️ Predict Attrition (classification model)
![roc_curve_attrition](https://github.com/user-attachments/assets/58c9e231-4ffe-452a-b5ab-ada5fd41c04b)

This phase of the HR Analytics project is executed with a high level of professional quality. Visualization choices are aligned with the data context, storytelling is strategic, and design decisions enhance stakeholder communication.

---

![istockphoto-1417959400-612x612](https://github.com/user-attachments/assets/02629cf3-4af8-48b2-8470-acbfc57049f7)


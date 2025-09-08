# Healthcare Dataset - Exploratory Data Analysis
- Author: Ahmed Essam
- Date: 9/8/2025
## Introduction
### In this project, we perform an exploratory data analysis (EDA) on a healthcare dataset that includes:
- Patient demographics
- Medical conditions
- Billing information
- Test results
- Admission and discharge dates
### The primary goals of this analysis are to:
- Uncover trends in healthcare utilization
- Detect anomalies in the data (e.g., outliers)
- Identify relationships between key attributes such as age, gender, admission type, and billing amount
## Tools Used
### Python:
- pandas
- matplotlib
- seaborn
## Dataset Overview
### The dataset is loaded from a .csv file.
### Key columns include:
- Demographics: Age, Gender, Blood Type
- Medical Info: Medical Condition, Insurance Provider, Medication, Test Results
- Billing Info: Billing Amount
- Date Fields: Admission & Discharge Dates
## Key Analytical Steps
## 1. Data Cleaning & Exploration
### Displayed dataset info, summary statistics, and missing values.
### Converted Admission Date and Discharge Date into:
- Day, Month, Year
- Weekday name
## 2. Outlier Detection & Distributions
- Analyzed columns: Age, Billing Amount
- Identified outliers using IQR method.
- Plotted histograms and boxplots for distribution insight.
## 3. Categorical Analysis
### Counted values and visualized distributions for:
- Gender
- Blood Type
- Medical Condition
- Insurance Provider
- Admission Type
- Medication
- Test Results
### Time-based analysis:
- Admissions and discharges across day, month, year, and weekday using line plots.
## Insights from Distribution Analysis
- Blood Types: Evenly distributed; A- most common, O- least common.
- Medical Conditions: Arthritis and Diabetes are most prevalent.
- Insurance: Cigna most used; Aetna least used.
- Admission Types: Elective most common.
- Medication: Lipitor most common; Penicillin least.
- Test Results: Majority are “Abnormal.”
- Admissions by Date:
  -- Highest in August
  -- Most admissions occurred on Thursday
  -- Peak year: 2020, reflecting pandemic impact.
- Discharges: Similar trends to admissions, with July and August highest.
## 5. Age Analysis by Category
### Computed median and standard deviation of age for:
- Gender
- Medical Condition
- Insurance Provider
- Admission Type
- Medication
- Test Results
### Findings:
- Age distributions are mostly homogeneous across all categories.
- No significant age difference among groups.
## 6. Billing Amount Analysis by Category
-Computed mean billing amount and its variability for all categories.
### Key Insights:
- Gender: Minimal difference between males and females.
- Medical Condition: Slight variations; Obesity had the highest average billing.
- Insurance Provider: Medicare had the highest billing.
- Admission Type: Elective had the highest mean billing.
- Medication & Test Results: Small differences overall.
- Date-Based Trends:
   -- Highest billing: October
   -- Highest weekday: Monday
   -- Lowest: Sunday and Friday
   -- Gradual increase in billing from 2019 to 2021
## 7. Category Comparisons (Cross-tabulation & Bar Charts)
### Compared:
- Gender vs Medical Condition, Insurance, Admission Type, Medication, Test Results
- Medical Condition vs Blood Type, Medication, Test Results, Admission Type
- Admission Type vs Test Results, Blood Type
### Highlights:
- Balanced distribution across genders.
- Medications and test results are evenly distributed across most conditions and admission types.
- Certain patterns like higher abnormal results in Elective admissions or higher urgent admissions in Diabetes patients were observed.
## 8. Hospital-Level Analysis
### Top 20 Hospitals by:
- Patient Count
- Average Billing Amount
- Median Age
### Insights:
- Hospital names like "Smith" and "Johnson" dominate.
- Top hospitals show higher billing and older patient demographics.
- All have billing averages above 51,000 and median age above 86, suggesting focus on elderly care.
## Conclusions
- The dataset reflects a balanced and realistic healthcare scenario, with well-distributed attributes across patients.
- No major disparities were found in age or billing across most categorical features.
- Some seasonal trends and pandemic effects (notably in 2020) are evident in the data.
-Admission and discharge patterns remain fairly stable across weekdays and months.
- Billing and age are not heavily influenced by demographic or medical factors in this dataset.
## Project Structure
├── healthcare_dataset.csv
├── healthcare_eda.ipynb / .py
└── README.md

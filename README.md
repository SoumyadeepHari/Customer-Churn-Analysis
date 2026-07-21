# Customer Churn Analysis

## Project Overview

Customer retention is often more cost-effective than acquiring new customers, making customer churn an important business problem.

In this project, I performed an exploratory data analysis (EDA) on a bank customer dataset to identify the characteristics most associated with customer churn. Using Python, I explored customer demographics, account information, and behavioral features to answer business-focused questions and uncover patterns that could help guide customer retention strategies.

---

## Objectives

This project aims to answer the following business questions:

- What is the overall customer churn rate?
- Does customer gender influence churn?
- Does geography influence churn?
- Does account activity status influence churn?
- Does age influence churn?
- Do older customers in Germany churn more than younger customers?
- Among inactive customers, does account balance influence churn?
- Does credit card ownership relate to churn?

---

## Dataset

The analysis uses **Churn_Modelling.csv**, which contains information about bank customers, including:

- Customer demographics (Age, Gender, Geography)
- Account information (Balance, Tenure, Number of Products)
- Customer engagement (Active Member, Credit Card Ownership)
- Target variable (Exited)

---

## Tools & Libraries

- Python
- Pandas
- Matplotlib
- Jupyter Notebook

---

## Sample Visualizations

The charts below highlight some of the key insights uncovered during the exploratory data analysis. They summarize the customer segments with the highest churn rates and support the business recommendations presented later in the project.

---

### 1. Churn Rate by Geography

<p align="center">
  <img src="images/churn_geography.png" width="700">
</p>

Germany has the highest customer churn rate (**32.44%**), nearly double that of France and Spain. This suggests that region-specific retention strategies may be required.

---

### 2. Churn Rate by Age Group

<p align="center">
  <img src="images/churn_age.png" width="700">
</p>

Customer churn increases with age and peaks in the **50–59** age group (**56.04%**), making this the highest-risk demographic.

---

### 3. Churn Rate by Activity Status

<p align="center">
  <img src="images/churn_activity.png" width="700">
</p>

Inactive customers churn at almost **twice the rate** of active customers, highlighting customer engagement as one of the strongest indicators of retention.

---

### 4. Churn Rate by Balance (Inactive Customers)

<p align="center">
  <img src="images/churn_balance.png" width="700">
</p>

Among inactive customers, those with positive account balances experience significantly higher churn than customers with zero balances, indicating a valuable customer segment that could benefit from targeted retention efforts.

---

## Methodology

The project follows a standard exploratory data analysis workflow:

1. **Data Inspection**
   - Checked dataset shape
   - Verified data types
   - Checked for missing values
   - Checked for duplicate records

2. **Data Cleaning**
   - Validated ranges for numerical columns
   - Verified binary variables
   - Renamed columns where appropriate
   - Created age groups and balance groups for deeper analysis

3. **Exploratory Data Analysis**
   - Calculated churn rates across different customer segments
   - Visualized trends using bar charts
   - Added written business insights after each analysis

4. **Summary of Findings**
   - Consolidated the most important business insights into actionable recommendations

---

## Key Findings

- **Overall churn rate:** **20.37%** (roughly one in five customers leave the bank)

- **Gender**
  - Female customers: **25.07%**
  - Male customers: **16.46%**

- **Geography**
  - Germany: **32.44%**
  - France: **16.15%**
  - Spain: **16.67%**

  Germany has nearly double the churn rate of the other two countries.

- **Customer Activity**
  - Active members: **14.27%**
  - Inactive members: **26.85%**

  Customer engagement appears to be strongly associated with retention.

- **Age**
  - Churn increases steadily with age and peaks at **56.04%** among customers aged **50–59**.

- **Germany + Age**
  - Customers aged **50–59** in Germany have the highest churn rate at **70.04%**.

- **Balance (Inactive Customers)**
  - Zero balance: **18.35%**
  - $1–50K balance: **51.43%**
  - $200K+ balance: **42.11%**

  Moderate- and high-balance inactive customers appear to be the highest-risk segments.

- **Credit Card Ownership**
  - With credit card: **20.81%**
  - Without credit card: **20.18%**

  Credit card ownership shows little to no relationship with customer churn.

---

## Business Insights

The analysis suggests that retention efforts should focus on:

- Customers located in Germany
- Customers aged 50–59
- Inactive customers
- Inactive customers with positive account balances

These segments consistently show the highest churn rates and may provide the greatest opportunity for targeted retention strategies.

---

## Limitations

This project focuses on exploratory analysis and identifies relationships rather than causation.

Some limitations include:

- No predictive machine learning model was built.
- Statistical significance testing was not performed.
- Business conclusions are limited to the available dataset.

Future work could include building classification models (Logistic Regression, Random Forest, XGBoost) to predict customer churn.

---


## What I Learned

Through this project I practiced:

- Data cleaning with Pandas
- Exploratory data analysis
- Data visualization with Matplotlib
- Translating analysis into business insights
- Organizing a complete analytics project using Git and GitHub

---

## License
This project is available for personal and educational use. Feel free to fork and adapt.

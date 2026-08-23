# 🛍️ Customer Shopping Behavior Analysis & Power BI Dashboard

## 📌 Project Overview

This project analyzes customer shopping behavior using SQL, Python, and Power BI.

The main objective is to understand customer purchasing patterns, revenue contribution, discount usage, customer segments, product performance, and subscription behavior.

The project starts with data cleaning and preparation in Python, followed by SQL-based analysis and finally an interactive Power BI dashboard for business insights.

---

## 🎯 Business Objectives

- Analyze overall customer purchasing behavior
- Identify top-performing products
- Analyze revenue by age group and category
- Understand discount usage and its impact on purchases
- Segment customers based on previous purchases
- Compare repeat buyers with non-repeat buyers
- Analyze customer subscription behavior
- Identify purchase frequency patterns
- Create an interactive dashboard for business decision-making

---

## 🛠️ Tools & Technologies

- **Python**
  - Pandas
  - NumPy
  - Data Cleaning
  - Data Transformation

- **SQL**
  - MySQL
  - Aggregate Functions
  - GROUP BY
  - HAVING
  - CASE WHEN
  - Subqueries
  - CTE
  - Window Functions

- **Power BI**
  - Data Modeling
  - DAX
  - KPI Cards
  - Donut Chart
  - Bar Chart
  - Column Chart
  - Slicers
  - Interactive Dashboard

- **GitHub**
  - Project Documentation
  - Version Control

---

## 📊 Dataset

The dataset contains customer shopping behavior information such as:

- Customer ID
- Age
- Gender
- Item Purchased
- Category
- Purchase Amount
- Location
- Size
- Color
- Season
- Review Rating
- Subscription Status
- Shipping Type
- Discount Applied
- Promo Code Used
- Previous Purchases
- Payment Method
- Frequency of Purchases
- Age Group
- Purchase Frequency Days

---

## 🧹 Data Cleaning & Preparation

Python Pandas was used for data cleaning and transformation.

### Major Steps

- Checked dataset structure
- Checked missing values
- Checked duplicate records
- Verified data types
- Created `age_group`
- Created `purchase_frequency_days`
- Prepared the cleaned dataset for SQL and Power BI analysis

Example transformation:

```python
frequency_mapping = {
    'Fortnightly': 14,
    'Weekly': 7,
    'Monthly': 30,
    'Quarterly': 90,
    'Bi-weekly': 14,
    'Annually': 365,
    'Every 3 months': 90
}

df['purchase_frequency_days'] = (
    df['frequency_of_purchases'].map(frequency_mapping)
)# customer_behavior_analysis

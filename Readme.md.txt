# Customer Churn Analysis (SQL + Power BI)

##  Overview
This project focuses on analyzing customer churn behavior using SQL and visualizing insights through Power BI.
The goal is to understand why customers churn, identify high-risk segments, and support data-driven retention strategies.
The analysis covers customer demographics, contract types, services used, revenue contribution, and churn reasons.

---

##  Problem Statement
Businesses want to understand:
- Which customers are more likely to churn?
- Key factors influencing churn (tenure, contract type, monthly charges)
- How churn trends vary across customer segments?

---

## Tools & Technologies
- Excel – Source dataset
- SQL Server - Data cleaning and analysis  
- Power BI – Interactive dashboards and visual insights  

---

## Data Preparation & SQL Approach
1. Data Exploration

Analyzed customer distribution by:
Gender
Contract type
State
Customer status
Calculated percentage contribution and revenue share
Identified churn impact on total revenue

2. Data Quality Checks
Checked null values across all key columns
Identified missing service and churn-related attributes

3. Data Cleaning & Transformation
Replaced NULL values using business logic:
Missing services → “No”
Missing deal types → “None”
Missing churn reasons/categories → “Others”
Inserted cleaned data into production table (prod_Churn)

4. SQL Views for Reporting
vw_ChurnData → Customers who Churned or Stayed
vw_JoinData → Newly Joined customers

These views are directly connected to Power BI

---

##  Key Insights
- Customers with month-to-month contracts showed higher churn
- Short tenure and higher monthly charges were strong churn indicators
- Long-term contracts had better retention rates

---

##  Conclusion
The dashboards help businesses identify churn drivers and focus retention efforts
on high-risk customer segments.

---

##  How to Run This Project

1.Import the churn dataset into SQL Server.
2.Execute SQL scripts for:
3.Data exploration
4.Data cleaning
5.View creation
6.Connect Power BI to SQL views (vw_ChurnData, vw_JoinData).
7.Refresh data and explore insights through the dashboard.

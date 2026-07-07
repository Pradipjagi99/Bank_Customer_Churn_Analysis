# <img width="42" height="42" alt="bank-teller" src="https://github.com/user-attachments/assets/81357c5b-6dec-4455-bc55-9f9846849d64" /> Bank Customer Churn Analysis

Identifying Customer Attrition Drivers and Retention Opportunities UsingSQL, Python,andPower BI

# Executive Summary

This comprehensive analysis examines customer attrition within a retail banking environment using a dataset of 10,000 customers. With a baseline churn rate of 20.38%, the project leverages SQL and Python for deep-dive exploratory data analysis (EDA) and Power BI for executive visualization. Key findings highlight a critical link between customer complaints and churn (99.5% correlation) and significant geographical risk in the German market.

## Business Problem & Objectives

Increased attrition is leading to direct revenue loss and diminishing customer lifetime value. This project aims to :
  - Identify primary churn drivers and high-risk segments.
  - Quantify financial impact to justify retention spend.
  - Develop strategic recommendations for cross-selling and service improvement

## 🎥 Demo

![Alt Text](https://github.com/Pradipjagi99/Bank_Customer_Churn_Analysis/blob/main/Bank_churn_analysis_demo.gif)

## ✨ Key Features

📌 **Data Visualization**: Interactive dashboards to provide clear insights into key metrics.

📌 **Trends Analysis**: Identifies performance trends over time.

📌 **Dynamic Reporting**: Easily filterable reports to focus on specific aspects of the dataset.

📌 **KPIs Monitoring**: Highlights the most critical performance indicators.

---

## 🛠️ Tools Used

**Python**: Exploratory Data Analysis using Python & Data Cleaning.

**SQL**: Business Analysis & Complex Querying.

**Power BI**: For data modeling, visualization, and dashboard creation.

---

## 🚀 Steps in Project

✔️ Requirement Gathering/Business Requirements
✔️ Exploratory Data Analysis
✔️ Data Import
✔️ Data Walkthrough  
✔️ Data Cleaning/Quality Check 
✔️ Data Connection
✔️ Data Analysis
✔️ Data Modeling  
✔️ Data Processing  
✔️ DAX Calculations  
✔️ Dashboard Lay outing  
✔️ Charts Development and Formatting  
✔️ Dashboard / Report Development  
✔️ Insights Generation

## 🧑‍💼 Business Problem Statement

Customer churn has increased and the bank is losing valuable customers. Management wants to identify key churn drivers and create data-driven retention strategies

## Questions Asked by Bank Manager

Revenue Questions:
- Which customer segments generate the highest revenue?
- Which segments are leaving the bank most often?
- How much balance is being lost due to churn?

Customer Retention Questions:
- What is the overall churn rate?
- Which age groups have the highest churn?
- Does geography affect churn?
- Does gender affect churn?
- Do inactive customers churn more?

Product Questions:
- Does number of products affect churn?
- Are credit card holders more loyal?
- Which card type has the highest churn?

Customer Satisfaction Questions:
- Does customer satisfaction impact churn?
- Do customers who complain leave more frequently?
- Which satisfaction score is associated with highest retention?

Risk Questions:
- What profile describes a typical churned customer?
- Which customers should be targeted first for retention campaigns?

---

## <img width="28" height="28" alt="image" src="https://github.com/user-attachments/assets/69cdf0b2-f650-4bb9-92a0-dd00b75d0154" /> Exploratory Data Analysis

## <img width="28" height="28" alt="image" src="https://github.com/user-attachments/assets/f1c36522-dba4-470f-94da-b308a20aad60" /> Data Import

- Data Loading: Imported the dataset using pandas.

![Description of the screenshot](https://github.com/Pradipjagi99/Bank_Customer_Churn_Analysis/blob/main/Images/Python/Screenshot%202026-07-07%20084006.jpg)

## <img width="28" height="28" alt="image" src="https://github.com/user-attachments/assets/9d0eeb64-72c3-4ba5-b79d-f37438f8fe5c" /> Data Walkthrough

- Rows: 10,000 
- Columns: 18
- Customer demographics: (Age, Gender, Geography)
- Identifiers: (RowNumber, CustomerId, Surname)
- Financial Profile: (CreditScore, Balance, EstimatedSalary)
- Account Activity: (Tenure, NumOfProducts, HasCrCard, IsActiveMember, Card Type, Point Earned)
- Behavior & Status: Exited (Churn status), Complain, Satisfaction Score

## <img width="28" height="28" alt="image" src="https://github.com/user-attachments/assets/c37e7042-4b39-450e-87bc-52ae0adb7f05" /> Data Cleaning/Quality Check

- Initial Exploration: Used df.info() to check structure and .describe() for summary statistics.

![Description of the screenshot](https://github.com/Pradipjagi99/Bank_Customer_Churn_Analysis/blob/main/Images/Python/Screenshot%202026-07-07%20084054.jpg)

![Description of the screenshot](https://github.com/Pradipjagi99/Bank_Customer_Churn_Analysis/blob/main/Images/Python/Screenshot%202026-07-07%20084213.jpg)

- Missing Data Handling: Checked for null values and imputed missing values in the Review Rating column using the median rating of each product category.

![Description of the screenshot](https://github.com/Pradipjagi99/Bank_Customer_Churn_Analysis/blob/main/Images/Python/Screenshot%202026-07-07%20084237.jpg)

- Unique values: Checking for unique values and if found duplicate correcting them.

![Description of the screenshot](https://github.com/Pradipjagi99/Bank_Customer_Churn_Analysis/blob/main/Images/Python/Screenshot%202026-07-07%20084258.jpg)










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

- Unique values: Checking for unique values 

![Description of the screenshot](https://github.com/Pradipjagi99/Bank_Customer_Churn_Analysis/blob/main/Images/Python/Screenshot%202026-07-07%20084258.jpg)

- Geography Distribution

![Description of the screenshot](https://github.com/Pradipjagi99/Bank_Customer_Churn_Analysis/blob/main/Images/Python/Screenshot%202026-07-07%20084349.jpg)

- Gender Distribution

![Description of the screenshot](https://github.com/Pradipjagi99/Bank_Customer_Churn_Analysis/blob/main/Images/Python/Screenshot%202026-07-07%20084416.jpg)

- Card Type Distribution

![Description of the screenshot](https://github.com/Pradipjagi99/Bank_Customer_Churn_Analysis/blob/main/Images/Python/Screenshot%202026-07-07%20084443.jpg)

- Churn Distribution

![Description of the screenshot](https://github.com/Pradipjagi99/Bank_Customer_Churn_Analysis/blob/main/Images/Python/Screenshot%202026-07-07%20084512.jpg)

- Check Duplicates
- CustomerId Duplicates

![Description of the screenshot](https://github.com/Pradipjagi99/Bank_Customer_Churn_Analysis/blob/main/Images/Python/Screenshot%202026-07-07%20084547.jpg)

---

## <img width="32" height="32" alt="exploratory-analysis" src="https://github.com/user-attachments/assets/8973903e-f2f7-4f19-9aff-7e71b01255e5" /> Exploratory Data Analysis (EDA)
- This is where the real business investigation begins.
    We will answer questions such as:
- Customer Churn
  - Which age group leaves most?
  - Which country has highest churn?
  - Do inactive customers churn more?
  - Does balance affect churn?
  - Do complaints drive churn?
- Product Analysis
  - Which products increase loyalty?
  - Which card type retains customers best?
- Executive Insights
  - At the end of EDA we'll create:
  - 10–15 business insights
  - KPI framework
  - SQL queries used in companies
  - Power BI dashboard layout
  - Management recommendation report
  - Future retention strategy report

Now we start answering management questions.

## Business Question #1

- Does Age Impact Churn?
- Are older customers leaving more often than younger customers

![Description of the screenshot](https://github.com/Pradipjagi99/Bank_Customer_Churn_Analysis/blob/main/Images/Python/Screenshot%202026-07-07%20084643.jpg)

- Visualization

![Description of the screenshot](https://github.com/Pradipjagi99/Bank_Customer_Churn_Analysis/blob/main/Images/Python/Screenshot%202026-07-07%20084724.jpg)

- Age Groups

![Description of the screenshot](https://github.com/Pradipjagi99/Bank_Customer_Churn_Analysis/blob/main/Images/Python/Screenshot%202026-07-07%20084751.jpg)

##  Business Question #2

- Does Geography Impact Churn?
- Which country is responsible for most customer losses?

![Description of the screenshot](https://github.com/Pradipjagi99/Bank_Customer_Churn_Analysis/blob/main/Images/Python/Screenshot%202026-07-07%20084850.jpg)

- Visualization

![Description of the screenshot](https://github.com/Pradipjagi99/Bank_Customer_Churn_Analysis/blob/main/Images/Python/Screenshot%202026-07-07%20084930.jpg)

##  Business Question #3

- Do Customer Complaints Drive Churn?
- Are customers leaving because they are unhappy?

![Description of the screenshot](https://github.com/Pradipjagi99/Bank_Customer_Churn_Analysis/blob/main/Images/Python/Screenshot%202026-07-07%20101337.jpg)

- Complaint Distribution

![Description of the screenshot](https://github.com/Pradipjagi99/Bank_Customer_Churn_Analysis/blob/main/Images/Python/Screenshot%202026-07-07%20101358.jpg)

- Visualization

![Description of the screenshot](https://github.com/Pradipjagi99/Bank_Customer_Churn_Analysis/blob/main/Images/Python/Screenshot%202026-07-07%20101425.jpg)

## Business Question #4

- Does Customer Satisfaction Affect Churn?
- Are dissatisfied customers leaving us?

![Description of the screenshot](https://github.com/Pradipjagi99/Bank_Customer_Churn_Analysis/blob/main/Images/Python/Screenshot%202026-07-07%20101455.jpg)

- Satisfaction vs Churn

![Description of the screenshot](https://github.com/Pradipjagi99/Bank_Customer_Churn_Analysis/blob/main/Images/Python/Screenshot%202026-07-07%20101516.jpg)

- Average Satisfaction

![Description of the screenshot](https://github.com/Pradipjagi99/Bank_Customer_Churn_Analysis/blob/main/Images/Python/Screenshot%202026-07-07%20101535.jpg)

- Visualization

![Description of the screenshot](https://github.com/Pradipjagi99/Bank_Customer_Churn_Analysis/blob/main/Images/Python/Screenshot%202026-07-07%20101558.jpg)

## Business Question #5

- Does Being an Active Member Reduce Churn?
- Are inactive customers leaving the bank?

![Description of the screenshot](https://github.com/Pradipjagi99/Bank_Customer_Churn_Analysis/blob/main/Images/Python/Screenshot%202026-07-07%20101638.jpg)

- Active Member vs Churn

![Description of the screenshot](https://github.com/Pradipjagi99/Bank_Customer_Churn_Analysis/blob/main/Images/Python/Screenshot%202026-07-07%20101700.jpg)

- Visualization

![Description of the screenshot](https://github.com/Pradipjagi99/Bank_Customer_Churn_Analysis/blob/main/Images/Python/Screenshot%202026-07-07%20101800.jpg)

## Business Question #6

- Does Account Balance Affect Churn?
- Are customers with higher balances more likely to leave?

![Description of the screenshot](https://github.com/Pradipjagi99/Bank_Customer_Churn_Analysis/blob/main/Images/Python/Screenshot%202026-07-07%20102454.jpg)

-  Boxplot

![Description of the screenshot](https://github.com/Pradipjagi99/Bank_Customer_Churn_Analysis/blob/main/Images/Python/Screenshot%202026-07-07%20102516.jpg)

- Create Balance Segments
- Churn by Balance Group

![Description of the screenshot](https://github.com/Pradipjagi99/Bank_Customer_Churn_Analysis/blob/main/Images/Python/Screenshot%202026-07-07%20102541.jpg)

## Business Question #7

- Does Number of Products Affect Churn?
- Do customers with more products stay longer?

![Description of the screenshot](https://github.com/Pradipjagi99/Bank_Customer_Churn_Analysis/blob/main/Images/Python/Screenshot%202026-07-07%20102607.jpg)

- Product vs Churn

![Description of the screenshot](https://github.com/Pradipjagi99/Bank_Customer_Churn_Analysis/blob/main/Images/Python/Screenshot%202026-07-07%20102629.jpg)

- Visualization

![Description of the screenshot](https://github.com/Pradipjagi99/Bank_Customer_Churn_Analysis/blob/main/Images/Python/Screenshot%202026-07-07%20103438.jpg)

## Business Question #8

- What causes churn?
- What does a typical churned customer look like?

![Description of the screenshot](https://github.com/Pradipjagi99/Bank_Customer_Churn_Analysis/blob/main/Images/Python/Screenshot%202026-07-07%20103459.jpg)

- Credit Card vs Churn

![Description of the screenshot](https://github.com/Pradipjagi99/Bank_Customer_Churn_Analysis/blob/main/Images/Python/Screenshot%202026-07-07%20103518.jpg)

- Card Type vs Churn

![Description of the screenshot](https://github.com/Pradipjagi99/Bank_Customer_Churn_Analysis/blob/main/Images/Python/Screenshot%202026-07-07%20103541.jpg)

- Average Metrics by Churn

![Description of the screenshot](https://github.com/Pradipjagi99/Bank_Customer_Churn_Analysis/blob/main/Images/Python/Screenshot%202026-07-07%20103604.jpg)

---

> [!NOTE]
> Click the dropdown list below for more information on SQL or Power BI.

---

<details>
<summary>SQL <img width="28" height="28" alt="image" src="https://github.com/user-attachments/assets/ee2f380f-d0fc-4898-a809-6d7d7572d768" /> </summary>

## 📂 Introduction to the Database

This project involves Bank Customer Churn analyzing.The dataset already contains a target variable (Exited) which means we can analyze why customers leave the bank and recommend actions to reduce churn. 

---    

## 🏗️ Database Setup

```sql
CREATE schema customer_churn;
USE customer_churn;
```

## 📂 Importing Data into MySQL Workbench

To work with the database, we first need to import the data from the `Customer-Churn-Records.csv` file into MySQL Workbench. Follow these steps:

1. **Open MySQL Workbench**:

   - Launch MySQL Workbench and connect to your database server.

2. **Select the Database**:

   - Use the `customer_churn` database by running:
     ```sql
     USE customer_churn;
     ```

3. **Go to the Import Section**:

   - Click on the "Server" menu and select "Data Import."

4. **Choose the CSV File**:

   - In the "Import" tab, choose the `Customer-Churn-Records.csv` file as the source.
   - Ensure the "Import Data from File" option is selected.

5. **Map the Table**:

   - Select the destination table (`customer_churn_records`).
   - Map the CSV columns to the corresponding table columns.

6. **Run the Import**:

   - Click on "Start Import."

---

## 📜 SQL Queries & Answers

### 1️⃣ Dataset Validation

**📝 Query:**

```sql
select count(*) as total_customers
from customer_churn_records;
```

**📊 Answer:**

![Description of the screenshot](https://github.com/Pradipjagi99/Bank_Customer_Churn_Analysis/blob/main/Images/SQL/Screenshot%202026-07-05%20112931.jpg)

---

### 2️⃣ Executive KPIs

**📝 Query:**

```sql
select 
	count(*) as total_customers,
    sum(Exited) as churned_customers,
    ROUND(SUM(Exited)*100.0/COUNT(*),2) AS churn_rate
from customer_churn_records;
```

**📊 Answer:**

![Description of the screenshot](https://github.com/Pradipjagi99/Bank_Customer_Churn_Analysis/blob/main/Images/SQL/Screenshot%202026-07-05%20113008.jpg)

---

### 3️⃣ Geography Analysis

**📝 Query:**

```sql
select
	Geography,
    count(*) as customers,
    round(avg(Exited)*100,2) as churn_rate
from customer_churn_records
group by Geography
order by churn_rate desc;
```

**📊 Answer:**
---

![Description of the screenshot](https://github.com/Pradipjagi99/Bank_Customer_Churn_Analysis/blob/main/Images/SQL/Screenshot%202026-07-05%20113120.jpg)

---

### 4️⃣ Age Analysis

**📝 Query:**

```sql
SELECT
    CASE
        WHEN Age BETWEEN 18 AND 30 THEN '18-30'
        WHEN Age BETWEEN 31 AND 40 THEN '31-40'
        WHEN Age BETWEEN 41 AND 50 THEN '41-50'
        ELSE '51+'
    END AS age_group,
    ROUND(AVG(Exited)*100,2) AS churn_rate
FROM customer_churn_records
GROUP BY age_group
ORDER BY churn_rate DESC;

```

**📊 Answer:**
---

![Description of the screenshot](https://github.com/Pradipjagi99/Bank_Customer_Churn_Analysis/blob/main/Images/SQL/Screenshot%202026-07-05%20113148.jpg)

---

### 5️⃣ Active Member Analysis

**📝 Query:**

```sql
SELECT
    IsActiveMember,
    ROUND(AVG(Exited)*100,2) AS churn_rate
FROM customer_churn_records
GROUP BY IsActiveMember;

```

**📊 Answer:**
---

![Description of the screenshot](https://github.com/Pradipjagi99/Bank_Customer_Churn_Analysis/blob/main/Images/SQL/Screenshot%202026-07-05%20113211.jpg)

---

### 6️⃣ Product Analysis

**📝 Query:**

```sql
SELECT
    NumOfProducts,
    COUNT(*) AS customers,
    ROUND(AVG(Exited)*100,2) AS churn_rate
FROM customer_churn_records
GROUP BY NumOfProducts
ORDER BY NumOfProducts;

```

**📊 Answer:**
---

![Description of the screenshot](https://github.com/Pradipjagi99/Bank_Customer_Churn_Analysis/blob/main/Images/SQL/Screenshot%202026-07-05%20113236.jpg)

---

### 7️⃣ Complaint Analysis

**📝 Query:**

```sql
SELECT
    Complain,
    COUNT(*) AS customers,
    ROUND(AVG(Exited)*100,2) AS churn_rate
FROM customer_churn_records
GROUP BY Complain;

```

**📊 Answer:**
---

![Description of the screenshot](https://github.com/Pradipjagi99/Bank_Customer_Churn_Analysis/blob/main/Images/SQL/Screenshot%202026-07-05%20113310.jpg)

---

### 8️⃣ Gender Analysis

**📝 Query:**

```sql
SELECT
    Gender,
    COUNT(*) AS customers,
    ROUND(AVG(Exited)*100,2) AS churn_rate
FROM customer_churn_records
GROUP BY Gender;

```

**📊 Answer:**
---

![Description of the screenshot](https://github.com/Pradipjagi99/Bank_Customer_Churn_Analysis/blob/main/Images/SQL/Screenshot%202026-07-05%20113339.jpg)

---

### 9️⃣ Balance Impact

**📝 Query:**

```sql
SELECT
    Exited,
    ROUND(AVG(Balance),2) AS avg_balance
FROM customer_churn_records
GROUP BY Exited;

```

**📊 Answer:**
---

![Description of the screenshot](https://github.com/Pradipjagi99/Bank_Customer_Churn_Analysis/blob/main/Images/SQL/Screenshot%202026-07-05%20113411.jpg)

---

- **📈 Key Insights**: Using SQL, we retrieve data that helps us answer questions such as:
  - Highest Risk Region : Germany (32.44% Churn)
  - Age-Related Attrition : Customers 51+ years old show 44.65% churn.
  - Complaint Impact : 99.5% of complaining customers churned.
  - Product Affinity : Lowest churn (7.6%) observed in 2-product segments.
  - Engagement Status : Inactive members churn at 26.87%

</details>

---

<details>
    <summary>Power BI <img width="28" height="30" alt="image" src="https://github.com/user-attachments/assets/1500083e-bdef-447f-9461-587caf8c5990" /> </summary>

# Bank Churn Analysis Dashboards 📊

This Power BI Dashboard provides a comprehensive analysis of Churned Customers and High-Risk Customer, focusing on churn rate by age group, average balance. The analysis leverages dynamic dashboards, interactive charts, and key performance indicators (KPIs) to identify trends and insights

# <img width="28" height="30" alt="data-analysis" src="https://github.com/user-attachments/assets/ba52b1af-a0ea-4893-903f-38f33a7e77ae" /> Dashboard Page 1: Executive Summary

![Description of the screenshot](https://github.com/Pradipjagi99/Bank_Customer_Churn_Analysis/blob/main/Images/Power%20Bi/Page1/Screenshot%202026-07-05%20105946.jpg)

## <img width="28" height="30" alt="image" src="https://github.com/user-attachments/assets/0d84fcf0-ed8b-4f45-8562-bfa71f9a93c5" /> KPI’s Requirements

**1. Total Customers** : The total count of different customers. 

**2. Churned Customers** : customers stop using the service.

**3. Churn Rate %** : percentage of customers stop using the service.

**4. Active Customers %** : Active users percentage.

**5. Avg Balance** : average of the balance amount.

**6. Complaint Rate %** : customers complaint percentage

---

![Description of the screenshot](https://github.com/Pradipjagi99/Bank_Customer_Churn_Analysis/blob/main/Images/Power%20Bi/Page1/Screenshot%202026-07-05%20110320.jpg)

---

## <img width="28" height="30" alt="image" src="https://github.com/user-attachments/assets/cfa5bf02-459a-4151-9654-1752bdb43139" /> Chart’s Requirements

- Churn Rate by Geography

![Description of the screenshot](https://github.com/Pradipjagi99/Bank_Customer_Churn_Analysis/blob/main/Images/Power%20Bi/Page1/Screenshot%202026-07-05%20110222.jpg)

- Customer Distribution by Geography

![Description of the screenshot](https://github.com/Pradipjagi99/Bank_Customer_Churn_Analysis/blob/main/Images/Power%20Bi/Page1/Screenshot%202026-07-05%20110158.jpg)

- Gender vs Churn

![Description of the screenshot](https://github.com/Pradipjagi99/Bank_Customer_Churn_Analysis/blob/main/Images/Power%20Bi/Page1/Screenshot%202026-07-05%20110112.jpg)

# <img width="28" height="30" alt="data-analysis" src="https://github.com/user-attachments/assets/ba52b1af-a0ea-4893-903f-38f33a7e77ae" /> Dashboard Page 2: Churn Drivers

![Description of the screenshot](https://github.com/Pradipjagi99/Bank_Customer_Churn_Analysis/blob/main/Images/Power%20Bi/Page2/Screenshot%202026-07-05%20110415.jpg)

# DAX Measures
- Churn rate
```
Churn Rate =
DIVIDE(
    SUM(customer_churn_records[Exited]),
    COUNT(customer_churn_records[CustomerId])
)
```

- Active Customer
```
Active Customer % =
DIVIDE(
    CALCULATE(
        COUNT(customer_churn_records[CustomerId]),
        customer_churn_records[IsActiveMember] = 1
    ),
    COUNT(customer_churn_records[CustomerId])
)  
```

- Complaint Rate
```
Complaint Rate =
DIVIDE(
    SUM(customer_churn_records[Complain]),
    COUNT(customer_churn_records[CustomerId])
)
```

- Total Balance Lost
```
Total Balance Lost =
CALCULATE(
    SUM(customer_churn_records[Balance]),
    customer_churn_records[Exited] = 1
)
```

- Average Balance
```
Avg Balance =
AVERAGE(customer_churn_records[Balance])
```

- Highest Risk Geography
```
Highest Risk Geography = "Germany"
```

- Highest Risk Age Group
```
Highest Risk Age Group = "51+"
```

- Female Churn Rate
```
Female Churn Rate =
CALCULATE(
    [Churn Rate %],
    customer_churn_records[Gender] = "Female"
)
```

- Germany Churn Rate
```
Germany Churn Rate =
CALCULATE(
    [Churn Rate %],
    customer_churn_records[Geography] = "Germany"
)
```

- High Balance Churn Rate
```
High Balance Churn Rate =
CALCULATE(
    [Churn Rate %],
    customer_churn_records[Balance] > 100000
)
```

## <img width="28" height="30" alt="image" src="https://github.com/user-attachments/assets/0d84fcf0-ed8b-4f45-8562-bfa71f9a93c5" /> KPI’s Requirements

**1. Highest Risk Age Group** : age group which are having highest churn rate are leaving service. 

**2. Highest Risk Geography** : region of customers leaving the service.

**3. Churn Rate %** : percentage of customers stop using the service.

**4. Highest Risk Driver** : drivers which are leading to lose customers.

---

![Description of the screenshot](https://github.com/Pradipjagi99/Bank_Customer_Churn_Analysis/blob/main/Images/Power%20Bi/Page2/Screenshot%202026-07-05%20110924.jpg)

---

## <img width="28" height="30" alt="image" src="https://github.com/user-attachments/assets/cfa5bf02-459a-4151-9654-1752bdb43139" /> Chart’s Requirements

- Complaint vs Churn

![Description of the screenshot](https://github.com/Pradipjagi99/Bank_Customer_Churn_Analysis/blob/main/Images/Power%20Bi/Page2/Screenshot%202026-07-05%20110533.jpg)

- Age Group vs Churn

![Description of the screenshot](https://github.com/Pradipjagi99/Bank_Customer_Churn_Analysis/blob/main/Images/Power%20Bi/Page2/Screenshot%202026-07-05%20110812.jpg)

- Active Member vs Churn

![Description of the screenshot](https://github.com/Pradipjagi99/Bank_Customer_Churn_Analysis/blob/main/Images/Power%20Bi/Page2/Screenshot%202026-07-05%20110632.jpg)

- Products vs Churn

![Description of the screenshot](https://github.com/Pradipjagi99/Bank_Customer_Churn_Analysis/blob/main/Images/Power%20Bi/Page2/Screenshot%202026-07-05%20110705.jpg)

- Balance Group vs Churn

![Description of the screenshot](https://github.com/Pradipjagi99/Bank_Customer_Churn_Analysis/blob/main/Images/Power%20Bi/Page2/Screenshot%202026-07-05%20110742.jpg)

# <img width="28" height="30" alt="data-analysis" src="https://github.com/user-attachments/assets/ba52b1af-a0ea-4893-903f-38f33a7e77ae" /> Dashboard Page 3: Customer Segmentation & Risk Profile





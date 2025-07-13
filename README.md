# Customer Churn Rate Analysis 📊

## Overview
This Power BI project focuses on analyzing **customer churn** for a business using various demographic and behavioral factors such as age, credit score, account balance, gender, activity status, and more. It provides clear visualizations to understand which customer segments are most at risk of churn.

---

## 🧹 Data Cleaning & Modeling

The raw data was cleaned and transformed in Power BI using Power Query Editor. The following steps were performed:

- Changed data types (e.g., Date → Text, Score → Whole Number).
- Renamed columns for clarity.
- Grouped continuous values (e.g., Age, Account Balance, Credit Score) into categories.

### 🔁 Reference Table Creation

Three new dimension/reference tables were created from the fact table (`Customer Data`) using **"Reference"** in Power Query:

1. **Account Balances Group**
   - Fields: `Account Balances ID`, `Account Balances`
   - Grouped by: Account balance ranges

2. **Age Group**
   - Fields: `Age Group ID`, `Age Group`
   - Grouped by: Age ranges (e.g., <20, 21–30, 31–40, etc.)

3. **Credit Score Group**
   - Fields: `Credit Scores ID`, `Credit Scores`
   - Grouped by: Credit score buckets (e.g., <=400, 401–500, 501–600, etc.)

These reference tables were linked back to the **Customer Data** table via respective foreign keys to form a **star schema** model.

---

## 📁 Project Structure

- **Customer Data**: Primary fact table with customer details and churn flag.
- **Account Balances Group**: Dimension table for account balance ranges.
- **Age Group**: Dimension table for age categories.
- **Credit Score Group**: Dimension table for credit score buckets.

All dimension tables have a 1-to-many relationship with the **Customer Data** table.

---

## 🔍 Key Insights

- **Total Customers**: 10,000  
- **Customers Lost**: 2,037  
- **Overall Churn Rate**: 20.37%

### Breakdown by Factors:

#### 🔢 Churn Rate by Credit Score
- Customers with very low credit scores (<=400) have the highest churn.

#### 🎂 Churn Analysis by Age Group
- Highest churn observed in the **31–40 age group**.

#### 🎯 Other Distributions:
- **Products**: Most customers own Product 2.
- **Country**: Fairly distributed across France, Germany, and Spain.
- **Gender**: Slightly more female customers (54.57%).
- **Activity**: Nearly equal split between active and inactive users.
- **Credit Card Ownership**: Majority own a credit card.

---

## 🛠 Tools & Technologies Used

- **Power BI Desktop**
- **DAX for measures (e.g., Churn Rate, Customers Lost, etc.)**
- **Power Query Editor** for cleaning, transformation, and reference creation
- **Data Modeling** using star schema

---

## 📸 Dashboard Preview

- **Data Model**  
  <img width="1005" height="698" alt="image" src="https://github.com/user-attachments/assets/38d24917-3990-4466-a98c-b7970b6e60ff" />


- **Churn Rate Dashboard**  
  <img width="1286" height="729" alt="image" src="https://github.com/user-attachments/assets/d06c6126-3bc0-4b30-a95b-a30d21ec7436" />


---

## 📌 Purpose
This project aims to:
- Identify churn-prone customer segments.
- Help businesses take proactive retention measures.
- Demonstrate skills in Power BI: cleaning, grouping, DAX, modeling, and dashboarding.

---

## 🤝 Contact
For any questions or collaboration opportunities, feel free to reach out!

---

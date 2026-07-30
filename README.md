# PhonePe--Analytics-Dashboard
An interactive Power BI dashboard analyzing PhonePe transactions, user demographics, DAX measures, and payment insights.



# 📊 PhonePe Analytics Dashboard (Power BI)

An interactive and comprehensive **Power BI Dashboard** analyzing transaction trends, user demographics, service breakdown, and key operational metrics for PhonePe ("Payment Insights, Powering Bharat").

---

## 📸 Dashboard Overview

| Dashboard Main View | Power BI Desktop Modeling & DAX |
| :---: | :---: |
| ![PhonePe Dashboard View](https://via.placeholder.com/800x450?text=PhonePe+Dashboard+Main+View) | ![Power BI Modeling View](https://via.placeholder.com/800x450?text=Power+BI+Desktop+Data+Model) |

---

## 📌 Project Overview & Key Features

This project provides end-to-end data analysis and visualization of PhonePe's transaction data. Key highlights include:

- **Key Performance Indicators (KPIs):**
  - **Total Transactions:** Overall count of transactions.
  - **Total Value (₹):** Aggregate monetary value across transactions (e.g., ₹44.51M).
  - **Unique Users / Total Users:** Count of active unique users in the platform.
  - **Success Rate (%):** Monitoring transaction success rates (e.g., 96.11%).
  - **MoM Growth Rates (%):** Month-over-Month percentage metrics for transactions and transaction value.

- **Visual Insights & Breakdowns:**
  - **Transactions Over Time:** Line/trend analysis showing transaction flow month by month.
  - **Age Segment Contribution:** Donut chart categorizing users across segments (**Millennials, Gen X, Gen Z, Boomers**).
  - **Service Transaction Value Analysis:** Bar chart visualizing transaction volume by service categories (**Loans, Money Transfer, Insurance, Recharge, etc.**).
  - **Top 5 Users:** Identifying key high-value users based on total transaction amount.
  - **Weekday vs. Weekend Usage:** Breakdown of user activity on weekdays vs. weekends.
  - **Interactive Slicers / Filters:** Filter data dynamically by **Month** and **Payment Status** (e.g., *Successful*, *Failed*).

---

## 📁 Data Model & Architecture

The project is modeled using Power BI's Data View and DAX measures.

### Tables & Relationships:
1. `All_Transactions` — Core fact table storing transaction details (`Transaction_ID`, `Service Type`, `Value`, `Status`, `Date`).
2. `All_Users` — Dimension table containing user profiles (`User_ID`, `Name`, `Age`, `Age Segment`, `Join_Date`).
3. `Date_Table` — Dedicated date hierarchy table (`Date`, `Day No`, `Month`, `Month No`, `Quarter`, `Weekday`, `Weekend`, `Year`).
4. `Measures` — Centralized DAX measure folder.

### Key DAX Measures Calculated:
- **`Total Transactions`**: Count/Sum of all user transactions.
- **`Total Transaction Value`**: `SUM(All_Transactions[Value])`
- **`Success Rate`**: `DIVIDE(Successful Transactions, Total Transactions, 0)`
- **`Total Trans MOM%`**: Month-over-Month growth percentage in transaction counts.
- **`Trans Value MOM%`**: Month-over-Month growth percentage in transaction value.
- **`Total Trans PM` / `Trans Value PM`**: Previous Month baseline calculations for comparative DAX modeling.

---

## 🛠️ Tech Stack & Tools Used

- **Business Intelligence Platform:** Power BI Desktop
- **Data Modeling:** Power BI Data Model, Star Schema
- **Calculations & Analytics:** DAX (Data Analysis Expressions)
- **Data Transformation:** Power Query Editor
- **Version Control:** Git & GitHub

---

## 🚀 How to Open & Run the Dashboard

1. **Clone the Repository:**
   ```bash
   git clone [https://github.com/Harshitsoni-1703/Phonepe-Analytics-Dashboard.git](https://github.com/Harshitsoni-1703/Phonepe-Analytics-Dashboard.git)

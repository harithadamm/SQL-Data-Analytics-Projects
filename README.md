# SQL-Data-Analytics-Projects

# Data Warehouse Sales EDA & Insights

## 📖 Executive Summary
This project explores a retail data warehouse dataset using SQL‑based exploratory data analysis (EDA).  
The dataset is structured in a **fact‑dimension model**, enabling analysis of customer behavior, product performance, regional sales, and profitability.  

The objective is to demonstrate how SQL EDA can uncover hidden patterns in a warehouse environment and translate them into **business insights** that drive strategic decisions.

---

## 🗂 Project Scope
This project involves:
- Performing **SQL exploratory data analysis (EDA)** on a retail data warehouse.  
- Investigating **sales trends, product concentration, customer loyalty, and regional performance**.  
- Applying **business storytelling** to communicate findings beyond raw queries.  
- Preparing insights that can be visualized in BI tools (Tableau/Power BI).  

---

## 📋 Project Requirements
- **Dataset Structure**:  
  <img src="https://github.com/harithadamm/asset-project/blob/main/Screenshot%201.png " width="400" /> 

- **Tools & Technologies**:  
  - SQL Server (SSMS) → EDA queries, joins, aggregations, window functions.  
  - Excel / Tableau → optional visualization of results.  

- **Skills Applied**:  
  - Data warehouse modeling (fact + dimension).  
  - SQL queries for aggregation, filtering, and trend analysis.  
  - Analytical storytelling to connect findings with business impact.  

---

## 📊 Key Insights
- **Sales Trends**: Revenue peaked during pandemic‑driven demand (2020) but declined steadily post‑2021, with seasonal recovery in Q4.  
- **Product Performance**: 70% of revenue concentrated in three products, creating dependency risk. Accessories grew in order share but remain <4% of revenue.  
- **Customer Loyalty**: Loyalty members contributed 55% of revenue in 2022, spending $35 more per order than non‑members.  
- **Regional Comparisons**: North America leads with highest AOV ($242), while EMEA showed late‑year growth in order share.  

---

## 🧮 SQL Exploratory Queries
Representative formulas and queries used in the analysis:

1. **Customer Growth Rate**  
   ```sql
   (COUNTD([CY Customers]) - COUNTD([PY Customers])) / COUNTD([PY Customers])

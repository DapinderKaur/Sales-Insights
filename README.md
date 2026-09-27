# Sales Insights

## 📌 Project Overview

**Project Type:** Guided Project

**Guidance:** This project was completed by following a guided tutorial. The project provided hands-on practice with SQL, data analysis, data validation, and Power BI dashboard development.

The objective of this project was to analyze sales data and transform it into meaningful business insights using SQL and Power BI.

The analysis focuses on revenue, sales quantity, profit margin, customers, products, and markets to understand overall sales performance and identify areas of improvement.

---

## 🛠️ Tools Used

- MySQL
- Power BI

---

## 🔄 Project Workflow

1. Imported the sales database into MySQL.
2. Explored the available tables and relationships between transactions, products, customers, markets, and dates.
3. Used SQL queries to understand the data and calculate key business metrics.
4. Performed data-quality checks, including identifying product codes present in transactions but missing from the product table.
5. Added missing product codes with an `Unknown` product type where required.
6. Analyzed revenue, sales quantity, profit margin, customers, products, and markets using SQL.
7. Connected the data to Power BI.
8. Created measures and visualizations for sales analysis.
9. Built an interactive Power BI sales insights dashboard.
10. Used SQL calculations to validate and cross-check dashboard results.

---

## 📊 Dashboard

The Power BI dashboard provides an overview of sales performance across different business dimensions, including:

- Revenue
- Sales Quantity
- Profit Margin
- Profit Margin %
- Sales by market
- Sales by customer
- Sales by product
- Year-over-year performance
- Product and market performance

### Dashboard Preview

#### Dashboard 1

![Sales Insights Dashboard 1](sales_insights_dashboard%281%29.png)

#### Dashboard 2

![Sales Insights Dashboard 2](sales_insights_dashboard%282%29.png)

#### Dashboard 3

![Sales Insights Dashboard 3](sales_insights_dashboard%283%29.png)

---

## 📈 Key Insights

### Overall Performance

- The dataset contains **338 products, 17 markets, and 38 customers**.
- In 2020 compared with 2019, **revenue decreased by 15.32%**, sales quantity decreased by **12.23%**, and profit margin decreased by **65.64%**.
- The decline in profit margin was substantially greater than the decline in revenue. For example, in February, revenue was approximately **27M in both years**, while profit margin decreased by **65.78%**.
- **Higher sales or revenue did not necessarily translate into a higher profit margin %**. This pattern was observed across markets, customers, and products.

### Market Analysis — 2020

- **Delhi NCR** generated the highest revenue at **78M**, contributing **54.7%** of total revenue, but its profit margin % was only **0.6%**.
- **Bhubaneshwar** generated the lowest revenue at **161.57K**, but had the highest profit margin % at **10.5%**.
- **Mumbai** had the highest profit margin contribution at **23.9%**.
- **Lucknow** was a loss-making market, with a profit margin % of **-2.7%**.
- **119 distinct products** were sold in Delhi NCR, compared with only **7** in Bhubaneshwar.

### Customer Analysis — 2020

- **Electricalsara Stores** generated the highest revenue (**65.64M**) and sales quantity (**100K**), but its profit margin % was only **0.4%**.
- **Electricalsbea Stores** had the highest profit margin % at **15.6%**, despite contributing only **0.0% of total revenue**.
- **6 customers** had negative profit margin %, indicating that sales to these customers resulted in overall losses.

### Product Analysis — 2020

- Of the **338 products**, only **197 had transactions in 2020**. Among these, **127 were profitable, 69 were loss-making, and 1 had zero profit**.
- **Prod318** generated the highest revenue contribution at **6.2% (8.79M)** and contributed **12.9% of total profit margin**.
- **Prod237** had the highest sales quantity (**43K**), but its profit margin % was **0.0%**, showing that high sales volume did not necessarily result in strong profitability.
- **Prod131 and Prod121** had the widest market reach, with each being sold in **9 markets**. Prod131 was profitable in **8 of those markets** and loss-making in **1**.
- **40 products** generated negative margins across all their active markets.

---

## 🗄️ SQL Analysis

SQL was used throughout the project for data exploration, validation, and business analysis.

The analysis included:

- Exploring the database tables
- Counting transactions, markets, products, and customers
- Calculating total revenue
- Comparing revenue between 2019 and 2020
- Analyzing monthly and yearly sales
- Analyzing sales by market
- Checking product availability across markets
- Identifying missing product codes
- Investigating product and market performance

The SQL analysis queries are available in:

`sales_insights_analysis.sql`

---

## 🧹 Data Quality Checks

During the analysis, product codes were identified in the transaction data that were not present in the product table.

These missing product codes were investigated and added to the product table with an `Unknown` product type where necessary.

This helped maintain consistency between the transaction and product tables before using the data for dashboard analysis.

---

## 📁 Files in This Repository

| File | Description |
|------|-------------|
| `Sales_Insights.pbix` | Power BI dashboard |
| `sales_insights_analysis.sql` | SQL queries used for data exploration, analysis, and validation |
| `sales_insights_database.sql` | SQL database dump containing the project database |
| `sales_insights_dashboard(1).png` | Dashboard preview - Page 1 |
| `sales_insights_dashboard(2).png` | Dashboard preview - Page 2 |
| `sales_insights_dashboard(3).png` | Dashboard preview - Page 3 |
| `README.md` | Project documentation |

---

## 🎯 Key Learning

This project provided hands-on practice with:

- SQL data exploration
- SQL aggregation and filtering
- Joining multiple tables
- Identifying and handling missing data
- Revenue and profit analysis
- Year-over-year comparison
- Power BI data modeling
- DAX measures
- Interactive dashboard development
- Validating Power BI results using SQL

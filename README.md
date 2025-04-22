# Brazilian E-Commerce Data Analysis Project

This project focuses on analyzing the Brazilian E-Commerce Public Dataset by Olist, covering the end-to-end data analysis pipeline: from data extraction, transformation, and loading (ETL), to exploratory data analysis (EDA), and visual insights using Power BI.

## 📁 Project Structure
data-analysis-project/
│
├── data/

│   ├── raw/                

│   │   └── olist_customers_dataset.csv

│   │   └── olist_geolocation_dataset.csv

│   │   └── olist_order_items_dataset.csv

│   │   └── olist_orders_dataset.csv

│   │   └── olist_products_dataset.csv

│   │   └── product_category_name_translation.csv

│   ├── processed/

│   │   └── category_sales.csv

│   │   └── cust_retention.csv

│   │   └── customer_state.csv

│   │   └── delivery_days.csv

│   │   └── order_sales.csv

│   │   └── state_sales.csv

│

├── notebooks/

│   ├── 01_ETL.ipynb

│   └── 02_EDA.ipynb

│

├── database/

│   └── cleaned_data.db

│

├── visualizations/

│   └── powerbi_report.pbix

│

├── README.md

## 📊 Project Overview

### 🎯 Objective
To understand customer behavior, sales distribution, and key performance metrics by analyzing historical e-commerce data in Brazil.

💼 Business Questions
This project aims to address the following business questions:
1. Order Trend: How has the total number of orders changed over time? Are there any seasonal patterns or spikes in customer activity?
2. Top Markets: Which Brazilian states have the highest customer base and revenue contributions?
3. Product Insights: Which product categories generate the most revenue, and how can we optimize product offerings?
4. Customer Behavior: How many customers are making repeat purchases? What does this say about loyalty?
5. Delivery Performance: What percentage of orders are delivered on time? Are there issues with delivery that impact customer satisfaction?

### 📦 Dataset
Source: Brazilian E-Commerce Public Dataset by Olist
Scope: Sept 2016 – Aug 2018
Tables used: Customers, Orders, Order Items, Products, Sellers, Payments, Reviews, Geolocation

### 🔄 01_ETL.ipynb
This notebook performs:
- Importing multiple CSV files
- Merging and joining relevant tables
- Handling missing data
- Feature engineering (e.g., delivery time, review score categories)
- Saving the cleaned and enriched dataset for further analysis

### 📈 02_EDA.ipynb
This notebook includes:
- Descriptive statistics of customers, products, and sellers
- Order trends over time
- Revenue analysis by product category
- Delivery performance insights
- Customer purchase behavior

### 📊 Power BI Dashboard (dashboard.png)
Key insights visualized:
- Order Trend: Monthly total orders from Sept 2016 to Aug 2018
- Top 5 States by Customers: SP dominates with over 40k customers
- Top Product Categories by Revenue: Health & Beauty, Watches & Gifts, etc.
- Contributing States by Sales: SP leads with 40% share
- On-Time Delivery Rate: 91.89%
- Repeat Customers: 252 customers have made more than 2 purchases
![Powerbi_report_page-0001](https://github.com/user-attachments/assets/53dcd194-b8b2-468c-b708-c22ce8258644)

### 🚀 Tools & Technologies
- Python (pandas, matplotlib, seaborn)
- Jupyter Notebook
- Power BI
- Git & GitHub

### 📌 Insights
- Sales are highly concentrated in specific states like SP.
- Customer retention is relatively low, suggesting room for loyalty improvements.
- Certain categories drive more revenue, helpful for marketing focus.
- Delivery performance is generally strong, but outliers exist.

### 🧠 Future Improvements
Build a predictive model for customer churn
Implement clustering for customer segmentation
Automate the ETL process using Python scripts or Airflow
Deploy interactive dashboards using tools like Streamlit

📊 E‑Commerce Sales & Customer Analytics Project
A complete end‑to‑end analytics solution built using PostgreSQL (Neon), SQL, and Power BI to analyze sales performance, customer behavior, product trends, and marketing effectiveness for a synthetic e‑commerce business.

This project demonstrates strong capabilities in data modeling, ETL, analytical SQL, segmentation, and dashboard design.


🚀 1. Project Overview
This project replicates a real‑world e‑commerce analytics workflow, covering:

Database design and relational modeling

Synthetic data generation using SQL

Data cleaning and transformation

KPI computation and analytical SQL

RFM customer segmentation

Interactive Power BI dashboard

Business insights and documentation

The objective is to showcase a complete analytics pipeline from raw data to insights.


🗂️ 2. Folder Structure
Code
Ecommerce-Analytics-Project/
│
├── sql/
│   ├── create_tables.sql
│   ├── insert_data.sql
│   ├── cleaning_transformations.sql
│   ├── analysis_queries.sql
│   └── rfm_segmentation.sql
│
├── powerbi/
│   ├── ecommerce_dashboard.pbix
│   └── dashboard_screenshots/
│       ├── full_dashboard.png
│       ├── kpi_section.png
│       ├── country_revenue.png
│       ├── category_revenue.png
│       ├── trend_chart.png
│       └── traffic_source.png
│
├── data/
│   └── sample_export.csv
│
└── docs/
    └── project_report.pdf

🛢️ 3. Database Schema
The project uses a clean, normalized relational schema with five core tables:

customers
customer_id

first_name, last_name

gender

country

email

created_at

products
product_id

product_name

category, subcategory

price, cost

orders
order id

customer id

order_date

payment_method

order_status

order_items
order_item_id

order_id

product_id

quantity

price

total_amount

customer_sessions
session_id

customer_id

session_start, session_end

traffic_source

device_type

This schema supports revenue analysis, customer segmentation, and marketing attribution.


🧹 4. Data Cleaning & Transformations
Data cleaning was performed using SQL scripts to ensure accuracy and consistency:

Standardized country names

Standardized gender values

Corrected negative or zero quantities

Fixed invalid price values

Recalculated total_amount

Removed duplicate customer emails

Corrected session_end timestamps

Standardized traffic source labels

Enforced referential integrity across all tables

All logic is available in:
sql/cleaning_transformations.sql


📈 5. Analytical SQL & KPIs
Key business metrics were computed using SQL:

Total Revenue

Total Orders

Total Customers

Average Order Value (AOV)

Repeat Customer Rate

Top Countries by Revenue

Revenue by Category

Top 10 Products

Monthly Revenue Trend

Traffic Source Performance

Queries are available in:
sql/analysis_queries.sql


🎯 6. RFM Customer Segmentation
RFM segmentation was implemented using SQL NTILE scoring:

Recency → last order date

Frequency → number of orders

Monetary → total spend

Customer segments include:

Champions

Loyal Customers

Big Spenders

Frequent Buyers

New Customers

At Risk

Regular Customers

Segmentation logic is available in:
sql/rfm_segmentation.sql


📊 7. Power BI Dashboard
The Power BI dashboard provides a comprehensive view of business performance:

Dashboard Components
KPI cards (Revenue, Orders, Customers, AOV)

Monthly revenue trend

Category‑wise revenue

Top 10 products

Top 5 countries

Traffic source breakdown

Device usage

RFM segmentation summary

Screenshots are available in:
powerbi/dashboard_screenshots/


🔍 8. Key Insights
Electronics and Home & Kitchen are the highest‑revenue categories.

Saudi Arabia and UAE lead in total revenue contribution.

Mobile devices dominate customer browsing sessions.

AOV remains stable across months, indicating consistent purchasing behavior.

A strong base of repeat customers drives long‑term revenue.

RFM segmentation highlights a healthy mix of Champions and Loyal Customers, with a smaller At Risk segment.


🛠️ 9. Tech Stack
PostgreSQL (Neon) – database, data generation, cleaning, analysis

SQL – transformations, KPIs, segmentation

Power BI – dashboard and visualization

GitHub – version control and documentation


📄 10. Documentation
A detailed project report is available in:
docs/project_report.pdf


🙌 Author
       Shikha Karan  
       E‑commerce Analytics | SQL | Power BI | Data Modeling
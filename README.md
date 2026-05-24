# 🛒 E-Commerce Analytics Platform

## 📌 Project Overview
This project implements an end-to-end E-Commerce Analytics Platform using Databricks, PySpark, Delta Lake, and SQL.

The solution follows the Medallion Architecture (Bronze → Silver → Gold) to ingest, clean, transform, and analyze e-commerce sales data. The final business-ready datasets are visualized through Databricks Dashboards to provide actionable insights into customer behavior, sales performance, product performance, and regional trends.

## 🎯 Business Objective

The objective of this project is to build a scalable analytics platform capable of:
- Ingesting raw e-commerce datasets
- Performing data cleansing and transformation
- Creating analytical fact tables
- Generating business KPIs
- Supporting dashboard-based decision making
- Demonstrating modern Data Engineering best practices

## 📂 Dataset

Dataset Used:

Brazilian E-Commerce Public Dataset by Olist

The dataset contains information related to:

- Customers
- Orders
- Order Items
- Products
- Payments
- Reviews
- Sellers
- Product Categories

## 🛠️ Technology Stack

| Technology | Purpose |
|------------|----------|
| Databricks | Data Platform |
| PySpark | Data Processing |
| Delta Lake | Storage Layer |
| SQL | Data Analysis |
| Databricks Dashboard | Business Reporting |
| GitHub | Version Control |

## 🥉 Bronze Layer

Raw datasets were ingested into Delta tables without major transformations.

Tables:
- bronze.customers
- bronze.orders
- bronze.order_items
- bronze.products
- bronze.payments
- bronze.reviews
- bronze.sellers
- bronze.geolocation
- bronze.category_translation

Purpose:

- Preserve source data
- Enable traceability
- Support reprocessing

---
## 🥈 Silver Layer

Data cleansing and enrichment performed.

Examples:

- Null handling
- Type casting
- Date conversions
- Derived columns
- Data quality improvements

Tables:
- silver.customers
- silver.orders
- silver.order_items
- silver.products
- silver.payments
- silver.reviews
- silver.sellers
- silver.category_translation

---
## 🥇 Gold Layer
Business-ready analytical models.

### Fact Table
#### gold.fct_sales

Contains sales transactions enriched with:

- Customer information
- Product information
- Payment information
- Revenue metrics
- Order details

---
## 📊 KPIs Developed
### Monthly Revenue Trend
Tracks revenue growth over time.

Table:
```sql
gold.kpi_monthly_revenue
```

---

### Revenue by State

Identifies top-performing customer regions.

Table:

```sql
gold.kpi_state_sales
```

---

### Revenue by Product Category

Analyzes category-level sales performance.

Table:

```sql
gold.kpi_category_sales
```

---

### Top Products by Revenue

Highlights best-selling products.

Table:

```sql
gold.kpi_top_products
```

---

## 📈 Dashboard Metrics

Executive KPIs:

- Total Revenue
- Total Orders
- Total Customers
- Average Order Value (AOV)

Visualizations:

- Monthly Revenue Trend
- Revenue by State
- Revenue by Category
- Top Products Analysis
  
## 🚀 Future Enhancements

Planned improvements:

- Incremental Data Loading
- Slowly Changing Dimension (SCD Type 2)
- dbt Integration
- Automated Data Quality Tests
- Workflow Orchestration
- CI/CD Pipeline
- Real-time Streaming Ingestion

## 📚 Learning Outcomes
Through this project I gained hands-on experience in:

- Medallion Architecture
- PySpark Data Transformations
- Delta Lake
- Fact Table Modeling
- KPI Development
- Dashboard Design
- GitHub Version Control
- End-to-End Data Engineering Workflows

## 👤 Author

Lakshika Bhagat
Data Analytics | Data Engineering |Python | PySpark | Delta Lake |Databricks | SQL | Databricks | git | github

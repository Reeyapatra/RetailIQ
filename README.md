# 🛒 RetailIQ
End-to-end cloud analytics engineering project built on **Snowflake**, featuring a star-schema data warehouse, automated SQL ETL pipeline, data validation framework, and Power BI dashboards for customer and product insights.

---

## Project Overview

This project designs and implements a scalable cloud data warehouse on Snowflake and delivers interactive Power BI dashboards to analyze sales, customer behavior, and product profitability.

It demonstrates modern analytics engineering practices including dimensional modeling, cloud warehousing, and business intelligence delivery.

---

## Key Deliverables
- Cloud-native data warehouse on Snowflake
- Star schema with fact and dimension tables
- SQL-based ETL & transformation pipeline
- Data quality and validation layer
- Power BI semantic model and dashboards
- End-to-end analytics workflow

---

## Technology Stack

### Cloud & Warehousing
- **Snowflake** (Cloud Data Warehouse)
- Snowflake SQL
- Virtual Warehouses
- Staging & Transformation Layers

### Data Engineering & Modeling
- Dimensional Modeling (Star Schema)
- ETL / ELT Pipelines
- Data Validation & Testing

### Analytics & Visualization
- Power BI
- DAX Measures
- Interactive Filters
- KPI Dashboards

---

## Architecture
Source Data
↓
Snowflake Staging Layer
↓
Transformation (SQL)
↓
Dimensions & Facts
↓
Power BI Semantic Model
↓
Business Dashboards
---
## Data Warehouse Design

The warehouse follows a star schema optimized for analytical queries:

### Fact Table
- Sales Fact (Revenue, Profit, Quantity, Discount)

### Dimension Tables
- Customer
- Product
- Date
- Geography
- Segment

This structure enables fast aggregations and scalable reporting.

---

## SQL Pipeline (Execution Order)

Run the following scripts in sequence on Snowflake:

1. `sql/01_CREATE_DATABASE_SCHEMA.sql`
2. `sql/02_STAGE_LOAD.sql`
3. `sql/03_DIMENSIONS_BUILD.sql`
4. `sql/04_FACTS_BUILD.sql`
5. `sql/05_VALIDATION_CHECKS.sql`
6. `sql/06_LOAD_DW.sql`

Each step is designed to be modular and reusable.

---

## Dashboards (Preview)

### Customer Insights
![Customer Insights](dashboards/Customer_Insights.png)

### Product Performance
![Product Performance](dashboards/Product_Performance.png)

### Shipping & Delivery Performance
![Shipping Performance](dashboards/Shipping_Performance.png)

### Sales Overview
![Sales Overview](dashboards/Sales_Overview.png)
---

## Key Business Questions Answered

- Which customer segments generate the highest revenue?
- How does Average Order Value (AOV) vary across segments?
- Which products drive profitability?
- How do repeat ordering patterns change monthly?
- Which regions contribute most to sales?

---

## Data Quality & Validation

Implemented automated checks for:

- Orphaned dimension keys
- Duplicate records
- Invalid measures
- Null critical attributes
- Negative revenue/profit values

Ensures reliability for business reporting.

---

## How to Reproduce

### 1. Snowflake Setup
- Create database and warehouse
- Configure roles and permissions
- Upload raw data to staging tables

### 2. Run ETL
Execute SQL scripts in `/sql` folder in order.

### 3. Connect Power BI
- Connect Power BI to Snowflake
- Import semantic model
- Refresh dashboards

---
## Professional Impact

This project demonstrates:

- Cloud data warehousing on Snowflake
- Analytics engineering workflows
- Dimensional modeling expertise
- BI development skills
- Production-style data validation
- End-to-end ownership

Aligned with modern data platforms used at FAANG and enterprise companies.

---



## Acknowledgments
- Snowflake Inc.
- Power BI Community
- Syracuse University iSchool

# CRM-ERP-Data-Integration-Using-a-Layered-Data-Warehouse
Building a Data Warehouse

# SQL-Datawarehouse-Project
Building a datawarehouse


🌐 Overview

This project represents a Data Warehouse architecture built using SQL Server, designed to collect, clean, and transform data from different sources like CRM and ERP systems into business-ready insights for reporting and analytics.

🧱 Architecture Layers

1. Sources

  -Data comes from CRM and ERP systems.

  -These are CSV files stored in folders like customer details, product info, and sales records.

2. Bronze Layer – Raw Data

  -This layer stores the raw data exactly as it is from the source.

  -Load Type: Batch or Full(Bulk load) load using stored procedures.

  -No transformations are done here.

  -Purpose: to preserve original data for auditing or reprocessing.

3. Silver Layer – Cleaned & Standardized Data

  -Here, data is cleaned and standardized.

  Transformations include:

  -Data cleansing (remove nulls, fix errors)

  -Data standardization (consistent formats)

  -Data normalization

  -Derived columns (like profit = revenue - cost)

  -Data enrichment (adding extra useful info)

  -This layer prepares data for business use.

4. Gold Layer – Business-Ready Data

  -Data here is transformed into business models for analytics.

Transformations:

  -Data integration (joining CRM & ERP data)

  -Aggregations (like total sales per month)

  -Applying business logic.

  Data Models: Star schema, flat tables, or aggregated tables.


📈 Consume Layer (Outputs)

  -The cleaned and modeled data is consumed by:

  -BI & Reporting tools – dashboards and reports.
 
  -Ad-hoc SQL Queries – for analysis by data analysts.

  -Machine Learning – predictive models using structured data.

🔁 Data Flow 

  -Data flows from CRM and ERP → Bronze Layer (raw tables) → Silver Layer (cleaned tables) → Gold Layer (fact and dimension tables).
  -CRM and ERP data → cleaned customer and product info → combined into dim_customers, dim_products, and fact_sales tables.

** This project shows how raw data from multiple systems is **

1. Collected (Bronze)


2. Cleaned and standardized (Silver)


3. Transformed into business insights (Gold)


4. Used for reports and analytics (Consume layer)







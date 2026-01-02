# Adidas Sales Data Analysis Project

##  Overview
This is an end-to-end data engineering and analytics project built using **Databricks** to analyze **Adidas US sales data for the years 2020 and 2021**.  
The project follows the **Medallion Architecture (Bronze → Silver → Gold)** and produces business-ready insights that are visualized using **Databricks Dashboards**.

All data processing (Bronze, Silver, and Gold layers) is implemented in a **single Databricks notebook** for clarity and learning purposes.

---

##  Tech Stack
- Databricks
- Apache Spark (PySpark)
- Delta Lake
- SQL
- Databricks Dashboards
- GitHub (version control)

---

##  Architecture
**Medallion Architecture**

- **Bronze Layer** – Raw data ingestion and schema enforcement  
- **Silver Layer** – Data cleaning, standardization, and validation  
- **Gold Layer** – Business-level aggregations and KPIs  
- **Dashboard** – Visualization of Gold layer insights  

---

##  Bronze Layer
**Purpose:** Store raw data in a reliable format

### Key Steps:
- Ingest raw Adidas sales CSV data
- Infer and enforce schema
- Convert raw data into Delta format
- Store data as Bronze Delta tables

---

##  Silver Layer
**Purpose:** Prepare clean and trustworthy data for analytics

### Key Steps:
- Column name standardization
- Data type corrections
- Null value identification and handling
- Corrupt record detection using business rules
- Separation of clean and corrupt records
- Duplicate record removal
- Validation of row counts after cleaning

---

##  Gold Layer
**Purpose:** Generate business insights and KPIs

### Gold-Level Outputs:
- Overall KPIs (Total Sales, Total Profit, Units Sold, Avg Price)
- Total sales by month
- Total sales by state
- Total sales by region
- Total sales by retailer
- Units sold by product category and gender
- Top performing cities by profit

---

##  Dashboard
An interactive dashboard is created using **Databricks Dashboards** on top of Gold Delta tables.

### Dashboard Highlights:
- KPI cards for high-level business metrics
- Sales trend analysis over time
- Regional and state-level sales performance
- Retailer-wise comparison
- Product category and gender analysis
- Top-performing cities by profit

Dashboard screenshots are included in this repository.

---

## 📁 Project Structure
<img width="585" height="379" alt="image" src="https://github.com/user-attachments/assets/caf145cd-1646-4a6d-8d94-502b0ce724c9" />





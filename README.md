# sql-data-warehouse-project
# 📊 Data Warehouse & Analytics Project

A complete **end-to-end Data Warehousing and Analytics project** demonstrating how raw business data can be transformed into actionable insights using **SQL Server and modern data architecture practices**.

This project implements the **Medallion Architecture (Bronze → Silver → Gold)** to build a structured data warehouse from raw CSV data sources and perform analytical reporting.

---

# 🚀 Project Overview

The goal of this project is to design and implement a **modern data warehouse solution** that consolidates sales data from multiple sources and transforms it into a **business-ready analytical model**.

The project covers the full data lifecycle:

- Data ingestion from source systems
- Data cleaning and transformation
- Dimensional data modeling
- Analytical reporting using SQL

This project demonstrates practical skills in:

- SQL Development
- Data Engineering
- Data Modeling
- ETL Pipeline Design
- Data Analytics

---

# 🏗️ Data Architecture

This project follows the **Medallion Architecture**, which organizes data into three layers for improved reliability, scalability, and analytical usability.

## Bronze Layer – Raw Data

- Stores **raw source data** exactly as received.
- Data is ingested from **CSV files (ERP and CRM systems)** into SQL Server.
- No transformations are applied in this layer.

Purpose:
- Maintain a **single source of truth**
- Preserve original data for auditing and reprocessing.

---

## Silver Layer – Cleaned & Transformed Data

This layer focuses on **data quality and preparation**.

Processes performed:

- Data cleansing
- Removing duplicates
- Standardizing formats
- Handling missing values
- Normalizing datasets
- Integrating ERP and CRM datasets

The output is **clean, reliable, and structured data** ready for analysis.

---

## Gold Layer – Business Ready Data

The Gold layer contains **analytical data models optimized for reporting**.

This layer implements a **Star Schema**, including:

- **Fact tables** for measurable business events (e.g., sales)
- **Dimension tables** such as:
  - Customers
  - Products
  - Dates
  - Regions

This structure enables **fast analytical queries and reporting**.

---

# 🔄 ETL Pipeline

The project implements a **structured ETL workflow**:

## Extract

- Data extracted from **ERP and CRM CSV files**

## Transform

Transformations performed in the **Silver Layer**:

- Data cleaning
- Standardization
- Deduplication
- Data integration
- Data validation

## Load

- Clean data is loaded into the **Gold Layer star schema**
- Optimized for analytical queries and reporting

---

# 📊 Analytics & Reporting

Using the **Gold Layer**, SQL queries were developed to generate insights such as:

## Customer Insights

- Customer purchasing behavior
- Top customers by revenue
- Customer segmentation

## Product Performance

- Best selling products
- Product revenue contribution
- Product sales trends

## Sales Trends

- Revenue trends over time
- Monthly and yearly performance
- Regional sales performance

These analytics support **data-driven decision making**.

---

# 🛠️ Technologies Used

| Tool | Purpose |
|-----|------|
| SQL Server Express | Data warehouse database |
| SQL Server Management Studio (SSMS) | Database management |
| SQL | Data transformation and analytics |
| Draw.io | Architecture and data modeling diagrams |
| Git & GitHub | Version control |
| CSV Datasets | Source data |

---

# 📂 Repository Structure

```
data-warehouse-project/
│
├── datasets/                   # Raw datasets (ERP and CRM CSV files)
│
├── docs/                       # Architecture and project documentation
│   ├── etl.drawio
│   ├── data_architecture.drawio
│   ├── data_catalog.md
│   ├── data_flow.drawio
│   ├── data_models.drawio
│   └── naming-conventions.md
│
├── scripts/
│   ├── bronze/                 # Raw data ingestion scripts
│   ├── silver/                 # Data cleaning & transformation
│   └── gold/                   # Star schema and analytical models
│
├── tests/                      # Data quality tests
│
├── README.md                   # Project documentation
├── requirements.txt            # Project dependencies
├── LICENSE
└── .gitignore
```

---

# 📌 Project Objectives

## Data Engineering

- Build a **modern data warehouse**
- Design **scalable ETL pipelines**
- Ensure **data quality and integration**

## Data Analytics

Generate insights into:

- Customer behavior
- Product performance
- Sales trends

These insights help stakeholders **make informed business decisions**.

---

# 📈 Skills Demonstrated

This project highlights expertise in:

- Data Warehouse Architecture
- ETL Pipeline Development
- SQL Query Optimization
- Dimensional Data Modeling
- Analytical Reporting
- Data Engineering Best Practices

---

# 📚 Dataset

The project uses datasets from two business systems:

- **ERP System**
- **CRM System**

Data is provided in **CSV format** and imported into SQL Server for processing.

---

# 📖 Documentation

Detailed project documentation is available in the **docs/** directory, including:

- Data architecture diagrams
- ETL workflow diagrams
- Data catalog
- Star schema design
- Naming conventions

---

# 📜 License

This project is licensed under the **MIT License**.

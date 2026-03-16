# Data Lakehouse for Fitness Classification Analytics

A graduation thesis project focused on designing and implementing a modern **Data Lakehouse** architecture for fitness data analytics, classification, and reporting.

This project demonstrates an end-to-end analytics workflow, from raw data ingestion to transformed analytical datasets and dashboard-ready outputs, using technologies commonly applied in data engineering and analytics roles.

---

## Project Overview

The goal of this project is to build a scalable and structured data platform for analyzing fitness classification data.

Using the **Fitness Classification** dataset from Kaggle, the system is designed to:

- ingest raw data into a centralized storage layer,
- clean and transform the data for analysis,
- organize data into structured layers,
- support downstream reporting and visualization,
- and provide a foundation for machine learning-based classification tasks.

This project reflects practical concepts from **data engineering**, **data analytics**, and **modern Lakehouse architecture**.

---

## Objectives

- Build an end-to-end **Data Lakehouse pipeline** for fitness classification analytics.
- Apply a layered data architecture for better data quality and usability.
- Process and transform data using **PySpark** and **SQL**.
- Store analytical data in modern formats such as **Parquet** and **Delta Lake**.
- Prepare data for dashboarding with **Power BI** or **Apache Superset**.
- Support future extensions such as predictive analytics and machine learning.

---

## Architecture Concept

The project follows a layered data architecture inspired by the **Bronze - Silver - Gold** pattern:

- **Bronze Layer**: raw ingested data from source files
- **Silver Layer**: cleaned, standardized, and validated data
- **Gold Layer**: business-ready analytical datasets for reporting and modeling

This approach improves data reliability, traceability, and reusability across analytics workflows.

---

## Tech Stack

- **Python**
- **SQL**
- **Apache Spark (PySpark)**
- **Delta Lake**
- **Parquet**
- **MinIO / AWS S3**
- **Power BI / Apache Superset**
- **Jupyter / Databricks Notebooks**

---

## Key Features

- Raw data ingestion from source files
- Data transformation and cleaning using PySpark
- Structured storage with Parquet / Delta Lake
- Layered modeling for analytics consumption
- Exploratory data analysis in notebooks
- Dashboard-ready outputs for business insights
- Foundation for future machine learning integration

---

## Project Structure

```text
data-lakehouse-fitness/
│
├── data/                    # Dataset files
│   ├── raw/                 # Raw source data
│   └── processed/           # Cleaned / transformed data
│
├── notebooks/               # Notebooks for EDA, transformation, and experiments
├── scripts/                 # Python / PySpark ETL scripts
├── sql/                     # SQL queries for transformation or analysis
├── reports/                 # Reports, screenshots, diagrams, and outputs
├── docs/                    # Additional documentation
│
├── requirements.txt         # Python dependencies
├── .gitignore               # Ignored files and folders
└── README.md                # Project documentation

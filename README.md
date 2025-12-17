# Retail Store Sales – Business Intelligence Project

## Overview
This project presents an **end-to-end Business Intelligence (BI) solution for retail / e-commerce sales**, covering data cleaning, transformation, and visualization. A **dirty transactional dataset** is processed using a Python-based ETL pipeline in **Google Colab**, producing a clean CSV that feeds an interactive dashboard built in **Google Looker Studio**.

The focus of the project is to demonstrate realistic BI workflows: working with low-quality data, structuring analytics-ready datasets, and delivering business insights through KPIs and dashboards.

## Dataset
- **Source**: Kaggle – Retail Store Sales (Dirty for Data Cleaning)
- **Domain**: Retail / E-commerce sales
- **Initial condition**: Missing values, inconsistent formats, noisy categorical fields, and duplicated records

This dataset resembles real-world retail data quality issues, making it suitable for BI and data analytics practice.

## Project Structure
├── data/
│ ├── dataraw/ # Original raw dataset from Kaggle
│ └── datacleansed/ # Cleaned, analytics-ready CSV
│
├── ETL/
│ └── retail_sales_etl.ipynb # Python ETL notebook (Google Colab)
│
├── Dashboard/
│ └── Looker_Studio_Link.txt # Google Looker Studio dashboard reference
│


## ETL Process (Python – Google Colab)
The ETL pipeline was developed and executed in **Google Colab**, using Python libraries such as pandas and numpy.

### Extract
- Loaded the raw retail sales CSV from the `data/dataraw` directory.

### Transform
- Handled missing and null values
- Standardized categorical variables (sales channels, payment methods, product categories)
- Parsed and validated date fields
- Removed duplicates and invalid records
- Created derived fields required for BI analysis

### Load
- Exported a **clean CSV dataset** to `data/datacleansed`, used as the single source of truth for reporting.

## KPIs Implemented
The cleaned dataset supports the following core BI KPIs:

- **Total Revenue**
- **Total Transactions**
- **Unique Customers**
- **Total Quantity Sold**
- **Average Ticket Sale**

These indicators provide a concise overview of sales performance and customer behavior.

## Dashboard (Google Looker Studio)
An interactive dashboard was built in **Google Looker Studio**, connected directly to the cleaned CSV.

### Visualizations
- **Total Sales by Channel**
- **Total Sales by Payment Method**
- **Sales by Product Category**
- **Sales Over Time**
- **Average Sale by Day of the Week**

The dashboard enables exploration of trends, channel performance, and purchasing patterns.

## Business Value
This BI solution supports:

- Monitoring overall commercial performance
- Identifying high-performing sales channels and product categories
- Understanding customer purchasing behavior
- Detecting temporal patterns to support marketing and operational decisions

## Tools & Technologies
- **Python (pandas, numpy)** – ETL and data cleaning
- **Google Colab** – ETL execution environment
- **CSV** – Analytics-ready data storage
- **Google Looker Studio** – BI dashboard and visualization

## Project Type
- Business Intelligence (BI)
- Retail / E-commerce Sales Analytics
- Data Cleaning & ETL

## Output
- Raw and cleaned datasets
- Reproducible Python ETL notebook
- Interactive BI dashboard in Google Looker Studio and a copy in PDF format

---
This project demonstrates a complete BI workflow: from raw, low-quality data to clean datasets and decision-ready insights.

└── README.md

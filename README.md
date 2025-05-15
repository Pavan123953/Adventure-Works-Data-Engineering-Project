# Adventure-Works-Data-Engineering-Project

🧠 Project Overview
This project demonstrates a complete, real-world Azure Data Engineering workflow built around a retail sales dataset. It covers the journey of raw transactional data — from ingestion and processing to advanced visualization — leveraging core services of the Azure ecosystem.

The pipeline is designed to automate data movement and transformation, generate business-ready insights, and support decision-making in a retail context.

🧾 Dataset Used
Source: Simulated Retail Sales Dataset (CSV/Parquet format)

Content: Includes order details like order ID, date, customer info, product category, sales amount, and region.

Volume: Designed for high-ingestion testing (GB-scale files)

Use Case: Derive regional performance, sales trends, and product profitability insights from the data

🛠️ Tech Stack / Skills Applied
Category	Tools / Skills
Data Ingestion	Azure Data Factory
Raw Data Storage	Azure Data Lake Gen2
Processing & Cleaning	Azure Databricks + PySpark + Delta Lake
Data Modeling / Storage	Azure Synapse Analytics (Dedicated SQL Pools)
BI & Reporting	Power BI (dashboards for region-wise performance, monthly sales, product KPIs)
DevOps & Control	GitHub, Git for version control and pipeline tracking

🔄 Workflow Architecture
Ingestion:
Data is pulled from local/online sources into Azure Data Lake Gen2 via ADF pipelines on a schedule.

Transformation:
Raw CSVs are processed in Databricks notebooks using PySpark. Null handling, currency normalization, and feature engineering (e.g., profit margin, discounted rate) are performed. Processed data is saved in Delta Lake format.

Loading & Analysis:
Cleaned datasets are loaded into Azure Synapse Analytics using PolyBase for querying and aggregation.

Reporting:
Power BI connects directly to Synapse, offering real-time business KPIs across regions, time, and product categories.

⭐ Features
End-to-End CI Pipeline: Orchestrated using Azure-native services

Delta Lake Reliability: Guarantees consistency and ACID transactions

Real-Time Refresh: BI dashboards reflect pipeline updates

Retail Insights: High-value views on revenue, profit, and customer trends

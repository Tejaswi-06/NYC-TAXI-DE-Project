# 🚕 NYC Taxi Data Engineering Project (Azure)

## 📌 Overview
This project presents an end-to-end data engineering pipeline built on Azure using the Medallion Architecture (Bronze → Silver → Gold). It focuses on ingesting NYC Taxi 2023 data from external sources using Azure Data Factory and transforming it into structured, analytics-ready datasets using Azure Databricks.

The pipeline is designed to support dynamic data loading through parameterized workflows and applies data cleaning, transformation, and aggregation techniques to produce reliable and optimized data for analysis.

---
## 🏗️ Architecture

The pipeline follows a layered approach:

- **Bronze Layer** – Raw data ingestion from external sources  
- **Silver Layer** – Data cleaning and transformation  
- **Gold Layer** – Aggregated and business-level insights  

---

## 🛠️ Tech Stack

- Azure Data Factory – Data ingestion & orchestration  
- Azure Data Lake Storage – Storage for Bronze, Silver, Gold layers  
- Azure Databricks – Data processing using PySpark & SQL  
- Delta Lake – Optimized storage format  

---

## 🔄 Workflow

### 1. Data Ingestion (Bronze Layer)

- NYC Taxi 2023 dataset ingested from external source  
- Parameterized pipeline with ForEach activity used for dynamic monthly loading  
- Data stored in Bronze layer  

---

### 2. Data Transformation (Silver Layer)

- Data cleaning (handling null values)  
- Schema validation and column selection  
- Data type conversions  
- Joining trip data with lookup datasets  
- Split trip datetime into year, month, and date  
- Prepared structured data for further processing  
- Basic visualization (pie chart) created for exploratory data analysis (EDA)  

---

### 3. Data Aggregation (Gold Layer)

- Transformed Silver data into curated datasets  
- Implemented Delta Lake for optimized storage  
- Created analytical outputs  
- Stored final data in Delta format for efficient querying  

---

## ⚙️ Key Features

- Automated data ingestion and orchestration using Azure Data Factory  
- Dynamic data loading using parameterized pipelines and ForEach loop  
- Data transformation and processing using Azure Databricks (PySpark & SQL)  
- Implementation of Medallion Architecture (Bronze, Silver, Gold layers)  
- Use of Delta Lake in Gold layer for optimized performance  

---

🏁 Conclusion

This project demonstrates the successful implementation of an end-to-end data engineering pipeline on Azure using the Medallion Architecture. Raw NYC Taxi data was ingested using Azure Data Factory with automated and parameterized pipelines, enabling efficient and scalable data loading.

Azure Databricks was used to perform data cleaning, transformation, and processing using PySpark, converting raw data into structured and meaningful datasets. The final data was stored in the Gold layer using Delta Lake, ensuring optimized storage and improved query performance.

Overall, this project showcases practical experience in building automated data pipelines, integrating Azure Data Factory with Azure Databricks, and applying modern data engineering practices for real-world analytics.

---

👤 Author

Tejaswi

---



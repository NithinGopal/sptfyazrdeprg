# Spotify End-to-End Azure Data Engineering Project

This project is an **end-to-end data engineering solution on Azure**, built to simulate real-world data ingestion, transformation, and analytics workflows. The objective was to design a scalable and automated data pipeline using multiple Azure services and best practices used in production systems.

---

## 🔍 Project Overview
The project focuses on building a complete data platform for analyzing Spotify data. It follows the **Medallion Architecture (Bronze–Silver–Gold)** model and demonstrates incremental, metadata-driven data processing using both batch and streaming techniques.

---

## ⚙️ Tech Stack
- **Azure Data Factory (ADF):** Pipeline orchestration, incremental and backfill ingestion, dynamic parameterization, and data movement.  
- **Azure Data Lake Storage Gen2:** Used to store raw (Bronze), cleansed (Silver), and curated (Gold) data layers.  
- **Azure SQL Database:** Acts as the source system for ingesting raw data.  
- **Azure Databricks (PySpark):** For transformation, cleaning, aggregation, and building **metadata-driven** pipelines with **Spark Structured Streaming** and **Autoloader**.  
- **Unity Catalog:** Centralized management for data governance and access control in Databricks.  
- **Delta Lake & Delta Live Tables:** For versioned, incremental, and efficient data processing.  
- **GitHub Integration:** For CI/CD and version control using Databricks Asset Bundles and branch-based workflows.

---

## 🧱 Architecture Highlights
- Implements **Medallion Architecture** — Bronze (raw ingestion), Silver (cleansed), and Gold (curated) layers.  
- Supports **incremental ingestion** with **backfilling** capability.  
- Uses **metadata-driven pipelines** with **Jinja2 templates**.  
- Demonstrates **Spark Structured Streaming** with **Autoloader** for real-time ingestion.  
- CI/CD enabled using GitHub and Databricks Asset Bundles.

---

## 📊 Data Modeling
- Developed **Star Schema** and **Slowly Changing Dimensions (Type 2)** for analytical models.  
- Transformed data stored as **Delta tables** in the Gold layer to support downstream BI and reporting.

---

## 🚀 Key Learnings
- Designing modular, reusable, metadata-driven data pipelines.  
- Configuring and integrating multiple Azure resources for scalable data solutions.  
- Building data transformation logic using **PySpark** and **Delta Live Tables**.  
- Applying CI/CD and version control best practices with **GitHub**.

---

## 📘 Project Flow
1. Data extracted from **Azure SQL DB** using **Azure Data Factory**.  
2. Loaded into **Azure Data Lake (Bronze layer)** as raw data.  
3. Processed and transformed using **Databricks (Silver layer)**.  
4. Modeled into analytical **Gold layer** tables using **Delta Live Tables**.  
5. Curated data exposed for downstream analytics and BI reporting.

---

**Tools Used:** Azure Data Factory | Databricks | PySpark | Azure SQL | Data Lake Gen2 | Unity Catalog | Delta Live Tables | GitHub  

💡 *This project strengthened my understanding of cloud-based data engineering, pipeline design, and modern ETL frameworks on Azure.*

# Azure Databricks & PySpark Data Engineering Project

## 📌 Project Overview
This repository showcases my hands-on experience with **Azure Databricks, Azure Data Factory, and PySpark**

The project focuses on building an **end-to-end data pipeline** using **Azure Databricks, Azure Data Factory, PySpark, and Delta Lake**, demonstrating skills in **data ingestion, transformation, and optimization**.

## 🏗️ Technologies Used
- **Azure Databricks** - Managed Spark environment
- **Apache Spark (PySpark)** - Distributed data processing
- **Delta Lake** - ACID transactions for data lakes
- **Azure Data Lake Storage (ADLS)** - Cloud-based storage
- **Azure Blob Storage** - Data storage and ingestion
- **Azure DevOps/GitHub** - Version control and CI/CD
- **Python & SQL** - Data transformations

## 🛠️ Project Architecture

![f1_architecture](https://github.com/user-attachments/assets/7a1ba4b3-fd8c-481a-8eeb-f5143bb51af3)

## 📂 Repository Structure
```
📁 formula1-pipeline
│── 📁 analysis/           # Short Analysis of data
│── 📁 includes/           # Common functions used and configurations
│── 📁 ingestion/          # All of the notebooks used to ingest data
│── 📁 raw/                # Raw data creation notebook
│── 📁 transformations/    # Notebooks for processing all of the raw data
│── 📁 utils/              # Incremental Load script
│── README.md              # Project overview and setup instructions
│── LICENSE                # License for the repository
```

## 🚀 Features Implemented
✅ Data ingestion from Azure Blob Storage using **PySpark**  
✅ Data transformation using **Spark SQL & DataFrames**  
✅ Storing and optimizing data using **Delta Lake**  
✅ Writing partitioned Parquet files for better performance  
✅ Handling schema evolution and ACID transactions  
✅ Performance tuning with **Spark optimizations**  
✅ **Automated pipeline orchestration with Azure Data Factory (ADF)**  
✅ **Triggers for scheduled and event-based execution**  

## 📈 Data Pipeline Overview
The project implements a **scalable data pipeline** following these steps:

1. **Data Ingestion**: Raw data is ingested from **Azure Blob Storage** using **Databricks Autoloader** or **Spark APIs**.
2. **Data Cleaning & Transformation**: Using **PySpark DataFrames**, data is transformed, deduplicated, and enriched.
3. **Data Storage & Processing**:
   - Processed data is written to **Delta Lake** in **Azure Data Lake Storage (ADLS)**.
4. **Incremental Processing**: Change Data Capture (CDC) is handled using **Merge into** statements in **Delta Lake**.
5. **Performance Optimization**: Caching, Bucketing, and AQE (Adaptive Query Execution) are implemented.
6. **Pipeline Orchestration & Triggers**:
   - Azure Data Factory **pipelines** automate data movement and transformation.
   - **Triggers** are configured for Tumbling Windows as all of the data is historical and no longer being updated
7. **Data Export**: Data is written to **Parquet files** and exposed to downstream analytics platforms.

This pipeline ensures **data reliability, scalability, automation, and efficiency** using best practices in **Apache Spark, Databricks, and Azure Data Factory**.

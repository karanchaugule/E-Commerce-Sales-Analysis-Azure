# Project: Brazilian E-Commerce Big Data Pipeline

## 📝 Overview

This project builds a modern data pipeline for Brazilian e-commerce analytics using Azure's big data ecosystem. It ingests data from MongoDB and SQL databases, transforms it using Azure services, and loads it into Synapse Analytics for business insights.

  
## 🧱 Architecture
![Architecture Diagram](https://github.com/JuhilMohadikar/Brazilian-E-Commerce-Big-Data/blob/main/Architecture%20Diagram.jpg)


## 🛠️ Tech Stack

| Component               | Technology                        |
|-------------------------|-----------------------------------|
| **Data Sources**        | SQL Database, MongoDB             |
| **Ingestion**           | Azure Data Factory                |
| **Raw Data Storage**    | Azure Data Lake Storage Gen2      |
| **Transformation**      | Azure Databricks (PySpark)        |
| **Data Enrichment**     | MongoDB Table Lookup              |
| **Transformed Storage** | Azure Data Lake Gen2              |
| **Analytics**           | Azure Synapse Analytics           |

## 🔁 Data Flow

1. **Ingestion**  
   - Azure Data Factory ingests data from SQL and other external sources into ADLS Gen2 (Raw Zone).

2. **Storage (Raw)**  
   - Data is initially stored in **Raw Zone** of ADLS Gen2.

3. **Transformation**  
   - Azure Databricks reads raw data from ADLS, performs cleaning, aggregation, and joins it with enrichment tables from MongoDB.

4. **Enrichment**  
   - Lookup/join operations are performed on data from MongoDB for additional business context.

5. **Storage (Transformed)**  
   - The enriched and processed data is saved to **Transformed Zone** in ADLS Gen2.

6. **Analytics & Visualization**  
   - Transformed data is queried from Synapse Analytics and visualized using Power BI or built-in dashboards.


**Key Highlights:**
- Scalable, cloud-native architecture
- Integration of structured and semi-structured data
- Use of modern data engineering tools for transformation and analytics
- Business intelligence through rich visualizations






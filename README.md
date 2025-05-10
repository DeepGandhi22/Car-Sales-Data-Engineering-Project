# Car Sale Data Engineering Project (Incremental Data Ingesion and Handling SCD Type 1 data)

## Project Overview

This project demonstrates the implementation of a **modern data pipeline architecture** using Azure Data Factory, Azure SQL Database, GitHub, and Databricks. It focuses on handling **incremental data ingestion** and managing **Slowly Changing Dimensions (SCD) Type 1** as part of the data transformation and modeling process.

---

## Key Features

- **Incremental Data Loading** from Azure SQL Database and GitHub using Azure Data Factory
- **Data Lakehouse Architecture** with Bronze, Silver, and Gold layers
- **Data Transformation** using Azure Databricks
- **SCD Type 1 Handling** for dimension table updates
- Creation of **Fact and Dimension Tables** for analytical reporting

---

## Architecture

The pipeline follows a structured medallion architecture:

![Untitled Diagram](https://github.com/user-attachments/assets/a347644c-e58a-43f9-a9b4-9c9ff46df453)

### Data Sources
- **Azure SQL Database**
- **GitHub Repositories**

### Data Pipeline
- Data is ingested incrementally using **Azure Data Factory**
- Raw data is stored in the **Bronze Layer** of the data lake
  
![initial](https://github.com/user-attachments/assets/8d225865-685b-4cc5-98dd-3261706ec7de)
![Incremental](https://github.com/user-attachments/assets/822794bb-deff-4945-ab24-1c3cd509626c)

### Data Transformation
- Data is cleansed and joined in the **Silver Layer** using **Azure Databricks**
- Advanced logic is implemented to handle **Slowly Changing Dimensions Type 1**
- Transformed data is modeled into **Fact** and **Dimension Tables**

![Final_workflow](https://github.com/user-attachments/assets/7e4a74da-a082-4316-9b23-ad5f061a4447)

### Final Output
- Curated, analytics-ready data is stored in the **Gold Layer**
- The data is now ready for visualization and reporting

---

## What I Learned

- Implementing **incremental ingestion strategies** in real-world pipelines
- Handling **SCD Type 1 logic** for maintaining up-to-date dimension records
- Efficient use of **Databricks notebooks and workflows**
- Integrating multiple Azure services to build a scalable data pipeline

---

## Tools & Technologies

- Azure SQL Database
- Azure Data Factory
- Azure Data Lake Storage
- Azure Databricks
- Delta Lake
- GitHub

---
## Conclusion

This project demonstrates a robust and scalable approach to modern data engineering. With incremental ingestion and SCD handling in place, the pipeline ensures both performance and accuracy in analytical datasets.


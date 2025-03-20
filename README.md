# Healthcare-Billing-Data-Pipeline


**📌 Introduction**
The Healthcare Billing Data Pipeline is designed to streamline the ingestion, transformation, and analysis of hospital claims, transactions, and patient billing data. The goal of this project is to provide a structured data pipeline for efficient revenue cycle management (RCM), helping hospitals track claims, payments, denials, and key financial metrics.

This project leverages:

Azure Data Lake (ADLS) for raw data storage
Databricks & PySpark for data processing
SQL databases for structured analytics

##  Overview of the Dataset

**Data Sources**
The data pipeline ingests data from multiple sources, including:
✅ Hospital EMR Data – Patient encounters, provider details, and billing transactions.
✅ Payor Claim Files – Insurance claim approvals, denials, and reimbursements.
✅ ICD-10 API Data – Standardized classification of diseases for billing.

**Data Coverage & Structure**
Covers multiple hospitals (Hospital A & Hospital B).
Organized into Landing → Bronze → Silver → Gold layers using Medallion Architecture.
Data is stored in Azure Data Lake Storage (ADLS) in Parquet format and processed into SQL tables.

**Data Processing in Databricks**
Convert raw data into structured, validated, and analytics-ready format.

✅ Bronze Layer → Converts raw CSV/JSON into Parquet format.
✅ Silver Layer → Standardizes patient, claims, and transactions data.
✅ Gold Layer → Aggregates data for KPI tracking & analytics.

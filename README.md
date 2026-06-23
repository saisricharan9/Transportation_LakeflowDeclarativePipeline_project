🚖 Transportation Data Engineering Project
Databricks LakeFlow Declarative Pipelines (SDP) | PySpark | Delta Lake | AWS S3 | Unity Catalog

--------------------------------------------------------------------------------------


📌 Project Overview

This project demonstrates an end-to-end Data Engineering solution built using Databricks LakeFlow Spark Declarative Pipelines (SDP) and the Medallion Architecture.

The project simulates a transportation company (Good Cabs) that faces delays in data delivery and relies on inefficient manual orchestration. The solution modernizes the platform by implementing automated data pipelines using Databricks LakeFlow Declarative Pipelines.

🎯 Business Objectives
Automate data ingestion and transformation
Reduce ETL code complexity
Eliminate manual orchestration
Support incremental processing
Improve data quality and trust
Deliver BI-ready datasets for regional managers
---------------------------------------------------------------------------------------
🛠️ Technology Stack
Technology	Purpose
Databricks LakeFlow SDP	Pipeline Orchestration
PySpark	Data Processing
Delta Lake	Storage Layer
AWS S3	Raw Data Storage
Unity Catalog	Governance & Security
Delta CDF	Change Data Capture
GitHub	Version Control

----------------------------------------------------------------------------------------------
📂 Medallion Architecture
🥉 Bronze Layer

Raw ingestion layer.

Responsibilities
Read source CSV files from S3
Preserve raw data
Track ingestion metadata
Capture corrupt records
Maintain auditability
Features
Schema Inference
Ingestion Timestamp
Source File Tracking
Delta Storage
🥈 Silver Layer

Business transformation layer.

Responsibilities
Data cleansing
Data standardization
Business rule implementation
CDC processing
Features
Auto CDC
Insert Handling
Update Handling
Delete Handling
Schema Evolution
🥇 Gold Layer

Analytics-ready layer.

Responsibilities
Business reporting
Aggregations
City-level reporting
KPI generation
Features
Denormalized datasets
Regional manager views
BI-ready tables
Optimized analytics queries
⚡ Key Features
🔄 Incremental Processing

Processes only new or changed records, significantly reducing runtime and compute costs.

🔄 Auto CDC

Automatically handles:

Inserts
Updates
Deletes

without writing custom merge logic.

🏛️ Unity Catalog

Provides:

Centralized governance
Access control
Data lineage
Metadata management
🤖 Automatic Orchestration

LakeFlow Declarative Pipelines automatically:

Resolves dependencies
Determines execution order
Optimizes pipeline execution

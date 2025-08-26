# SuperCafe ETL Pipeline – Repository Overview

## Overview
The SuperCafe ETL Pipeline is a full-cycle data solution designed to provide actionable analytics on customer transactions and business trends.

This project began as a **group project during my data engineering bootcamp**, initially deployed on AWS. The original implementation allowed the team to practice event-driven ETL, AWS Lambda, S3, EC2, and Redshift integration.

I have now decided to **migrate the project to Microsoft Azure** to gain hands-on experience with Azure services, such as **Azure Data Factory**, **Azure SQL**, and **Databricks**, while reusing most of the existing ETL code.

The pipeline extracts, transforms, and loads (ETL) transaction data from CSV files into a structured database, powering dashboards and business intelligence insights.

---

## Repository Structure

- **AWS/** – Original deployment on AWS
  - **sprint_1/** – Sprint 1 files, data, scripts, documentation
  - **sprint_2/** – Sprint 2 files, data, scripts, documentation
  - **sprint_3/** – Sprint 3 files, data, scripts, documentation

- **Azure/** – Adapted deployment for Microsoft Azure
  - **src/** – ETL source code adapted for Azure
  - **data/** – Sample or processed data
  - **docker/** – Docker/Docker Compose configs for Azure setup
  - **README.md** – README specific to Azure deployment


- **AWS folder**: Contains sprint-wise breakdown of the ETL development, infrastructure setup, and dashboard integration.  
- **Azure folder**: Contains the ETL pipeline adapted for Azure services. Since most ETL code is reused, this folder focuses on adaptations and connection updates rather than incremental development.

---

## Purpose
This repository serves to:

1. Provide a full ETL solution for SuperCafe across multiple cloud providers.  
2. Demonstrate best practices in cloud-based ETL pipeline design.  
3. Enable understanding, running, and extending the pipeline on either AWS or Azure.

---

## Key Highlights
- **Multi-cloud readiness**: Supports both AWS and Azure environments.  
- **Reusable ETL code**: Core Python scripts are mostly cloud-agnostic.  
- **Data normalization**: Transactions, products, and branch data are structured to avoid duplicates.  
- **Containerization**: Docker and Docker Compose are used for local testing.  
- **Monitoring & dashboards**: Grafana dashboards provide analytics and visualization (AWS version implemented; Azure integration planned).  

---

## Next Steps
- Complete Azure Data Factory pipelines and orchestrate ETL jobs.  
- Validate ETL end-to-end with Azure SQL/Synapse and Blob Storage.  
- Expand Databricks integration for advanced transformations or analytics.  
- Maintain and version both AWS and Azure deployments separately for clarity.  

---

## Notes
- **AWS Folder**: Sprint-based documentation and development history.  
- **Azure Folder**: Adaptation-focused with minimal code changes.  
- Each cloud deployment should have its **own README** to document specific setup, scripts, and configurations.
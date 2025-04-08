# 💳 Credit Card Transactional Analysis for Fraud Risk

This project is focused on building a real-time data pipeline for analyzing credit card transactions and detecting potential fraud. It leverages scalable data engineering tools and services on **Google Cloud Platform (GCP)** using **PySpark**, **Airflow**, and **CI/CD with GitHub Actions**.

## 🚀 Project Overview

The pipeline ingests daily credit card transaction files and performs fraud risk calculations using custom business logic and transformations. The processed data is then loaded into BigQuery for analytics and monitoring.

## 🧰 Tech Stack

- **Language & Frameworks**: Python, PySpark  
- **Orchestration**: Apache Airflow (GCP Composer)  
- **Data Processing**: GCP Dataproc Serverless  
- **Data Storage**: Google Cloud Storage (GCS), BigQuery  
- **CI/CD**: GitHub Actions  
- **Version Control**: Git, GitHub  

## 🛠️ Key Features

- Static table creation in **BigQuery** to store card holder information  
- Ingest daily transactional JSON files from **Google Cloud Storage**  
- Process and validate data using **PySpark** on **Dataproc Serverless**  
- Perform fraud detection calculations and data transformations  
- Trigger PySpark job using **Airflow DAG** when new files arrive  
- Archive processed files in a separate GCS folder  
- Deploy Airflow DAGs and PySpark scripts automatically via **GitHub Actions CI/CD pipeline**


## 🧪 How It Works

1. **Trigger**: Airflow DAG is triggered when new transaction files are detected in **GCS**  
2. **Read**: PySpark script reads card holder data from **BigQuery** and transactional data from **GCS**  
3. **Transform**: Business rules and validations are applied for fraud risk scoring  
4. **Load**: Final data is written to **BigQuery** tables  
5. **Archive**: Processed transaction files are moved to an archive folder  
6. **CI/CD**: GitHub Actions deploy updated scripts and DAGs automatically to the cloud


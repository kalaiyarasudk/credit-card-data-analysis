# credit-card-data-analysis

Created a static table in BigQuery to store Card Holders information.
• Developed a PySpark script to read Card Holders data from BigQuery and daily transactional JSON files from Google Cloud Storage.
• Built a PySpark application with data validations, transformations, and fraud risk calculation logic.
• Designed an Airflow DAG using GCP Composer to detect new transactional files in Cloud Storage, trigger a Dataproc Serverless
PySpark job, and move processed files to an archive folder.
• Built a GitHub Actions workflow to automate deployment of Airflow DAG and PySpark application files to Google Cloud Storage.

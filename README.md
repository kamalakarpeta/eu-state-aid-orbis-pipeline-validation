# EU State Aid Data Pipeline with Data Validation and Standardization (Moody's Project)

**Description:**

This project, developed at Moody's, automates the integration of EU State Aid grant data into the Orbis database, enhancing analysis of grant recipients. It includes automated CSV export from the EU State Aid website, robust data validation, profiling, and standardized data ingestion, significantly improving data quality and team efficiency.

## Project Overview

This project streamlines the extraction, processing, and integration of EU State Aid data to enhance Moody's analysis and reporting. The key components are:

1.  **Automated CSV Export (Selenium):**
    * Automates CSV export from the EU State Aid website using Selenium.
    * Handles form submissions and website changes for reliable data extraction.
2.  **SharePoint CSV Storage & Transfer:**
    * Stores exported CSV files in a SharePoint folder.
    * Transfers files to AWS S3 using `office365-rest-python-client` and boto3.
3.  **AWS S3 Storage:**
    * Provides scalable storage for raw CSV files.
4.  **AWS Databricks Processing (PySpark):**
    * Processes CSV data in AWS Databricks with PySpark.
    * Performs data cleaning, transformation, and fuzzy matching.
    * Enriches data with Orbis database information.
5.  **Orbis Database Integration:**
    * Loads processed data into the Orbis database via SQL or API.
    * Maintains data integrity and updates grant information.
6.  **Data Validation (Great Expectations):**
    * Implements robust data validation to identify and rectify discrepancies.
    * Defines expectations, runs checks, and generates quality reports.
7.  **Data Profiling (Pandas Profiling):**
    * Profiles data to identify issues like missing values and inconsistencies.
8.  **Standardized Data Ingestion Template:**
    * Streamlines ingestion processes for consistency and efficiency.
9.  **Data Lineage Tracking:**
    * Tracks data transformations for integrity and traceability.
10. **Data Visualization (Power BI or Orbis Platform):**
    * Visualizes integrated data for Moody's analysis.

## Architecture

EU State Aid Website (Selenium) --> Email (CSV Attachment) --> Power Automate --> SharePoint Folder --> AWS Lambda/Python Script --> AWS S3 --> AWS Databricks (PySpark) --> Orbis Database --> Power BI/Orbis Platform

## Technologies

* **Automation & Web Scraping:**
    * Selenium (website automation)
    * Power Automate (email attachment handling)

* **Python:**
    * `office365-rest-python-client` (SharePoint API)
    * boto3 (AWS S3)
    * fuzzywuzzy (matching)
    * Beautiful Soup (web scraping)
    * Requests (HTTP requests)
    * Pandas (data manipulation)

* **AWS:**
    * AWS Lambda (serverless compute) or EC2 (virtual server)
    * AWS S3 (object storage)
    * AWS Databricks (PySpark processing)

* **Databricks:**
    * PySpark (distributed data processing)

* **Database:**
    * Orbis Database (SQL/API)

* **Visualization:**
    * Power BI
    * Orbis Platform

* **Orchestration:**
    * Apache Airflow

* **Validation:**
    * Great Expectations

* **Profiling:**
    * Pandas Profiling

* **Containerization:**
    * Docker

* **Version Control:**
    * Git

## Setup and Installation

1.  **AWS Setup:**
    * Create AWS account, S3 bucket, and Databricks workspace.
    * Configure IAM roles for access.

2.  **SharePoint Setup:**
    * Ensure access and credentials.

3.  **Orbis Setup:**
    * Ensure database/API access.

4.  **Python Dependencies:**

    ```bash
    pip install selenium office365-rest-python-client boto3 fuzzywuzzy great_expectations pandas_profiling
    ```

5.  **Databricks Setup:**
    * Mount S3 and create PySpark notebook.

6.  **Lambda/EC2 Setup:**
    * Configure for file transfer to S3.

7.  **Selenium Setup:**
    * Install webdriver and Selenium.

8.  **Airflow Setup:**
    * Install and configure Airflow.

9.  **Docker Setup:**
    * Install and configure Docker.

10. **Power Automate Setup:**
    * Create a Power Automate flow to monitor the email inbox for CSV attachments.
    * Configure the flow to save attachments to the specified SharePoint folder.
    * Ensure the Power Automate flow has the necessary permissions to access the email inbox and SharePoint folder.

## Usage

1.  Configure credentials for AWS, SharePoint, Orbis, and email.
2.  Run the Selenium script to export CSV files from the EU State Aid website.
3.  Ensure the Power Automate flow is active and monitoring the email inbox for CSV attachments.
4.  Verify that Power Automate has successfully saved the CSV attachments to the SharePoint folder.
5.  Run the AWS Lambda function or Python script to transfer files from SharePoint to S3.
6.  Process data in Databricks using the PySpark notebook.
7.  Load the processed data into the Orbis database using SQL or the API.
8.  Visualize the integrated data using Power BI or the Orbis platform.
9.  Schedule the processes using Apache Airflow or AWS services (CloudWatch Events/EventBridge, Databricks Jobs).
10. Run Great Expectations validation checks on the data.
11. Run Pandas Profiling to analyze data quality.

## Contributing

Internal Moody's project, contributions managed internally.

## License

Internal Moody's use.

**Contact:**

* LinkedIn: [URL](https://www.linkedin.com/in/kamalakarpeta/)

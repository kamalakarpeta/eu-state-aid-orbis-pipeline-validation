# EU State Aid Data Pipeline with Data Validation and Standardization

**Description:**

Developed an automated data pipeline to scrape EU State Aid grant data from the official EU website and integrate it into the Orbis database, a comprehensive repository of over 500 million private company profiles. This project significantly enhanced the Orbis platform by providing users with critical information on which companies have received public grants from the European Union. Furthermore, this project included the implementation of robust data validation, profiling, and the creation of a standardized data ingestion template, designed to improve data quality and team efficiency.

**Key Technologies:**

* Python (Beautiful Soup, Requests, Pandas)
* SQL (PostgreSQL, Orbis Database)
* Data Pipeline Orchestration: **Apache Airflow**
* Data Validation: **Great Expectations**
* Data Profiling: **Pandas Profiling**
* Version Control: **Git**
* Containerization: **Docker**

**Project Overview:**

* **Web Scraping:** Automated the extraction of EU State Aid grant data from the official website using Python's Beautiful Soup and Requests libraries.
* **Data Cleaning and Transformation:** Implemented data cleaning and transformation processes to ensure data consistency and accuracy.
* **Data Validation:** Integrated robust data validation using **Great Expectations** to identify and rectify data discrepancies before ingestion. This involved defining data expectations, running validation checks, and generating data quality reports.
* **Data Profiling:** Conducted thorough data profiling using **Pandas Profiling** to assess data quality and identify potential issues, such as missing values, outliers, and data type inconsistencies.
* **Standardized Data Ingestion Template:** Developed a comprehensive template to streamline data ingestion processes for the team, promoting consistency and efficiency. This template included guidelines for data extraction, transformation, validation, and loading, ensuring adherence to best practices.
* **Data Ingestion:** Successfully ingested the validated and profiled data into the Orbis database, enriching company profiles with grant information.
* **Data Lineage Tracking:** Implemented mechanisms to track data lineage, ensuring data integrity and traceability throughout the pipeline. This involved logging data transformations and dependencies, providing transparency and accountability.
* **Containerization:** Packaged the application into Docker containers to ensure consistent deployment across different environments.
* **Orchestration:** Used Apache Airflow to schedule, monitor, and manage the data pipeline, ensuring reliable and automated data processing.

**Key Achievements:**

* **Improved Data Accuracy:** Implemented robust data validation processes using Great Expectations, resulting in a significant reduction of data errors during ingestion.
* **Enhanced Team Efficiency:** Developed and deployed a standardized data ingestion template, streamlining workflows and reducing onboarding time for new team members.
* **Enriched Orbis Data:** Successfully integrated critical EU State Aid grant data into the Orbis platform, providing valuable insights to users.
* **Scalable Data Pipeline:** Built a scalable and maintainable data pipeline capable of handling large volumes of data and adapting to evolving data sources.
* **Data Quality Enhancement:** Proactively identified and addressed data quality issues through comprehensive profiling using Pandas Profiling, improving the overall reliability of the Orbis database.
* **Standardization:** Created a standard for data ingestion that was used by the entire data team, improving team consistency.
* **Automation:** Automated the data pipeline using Airflow, reducing manual effort and ensuring timely data updates.

**Project Context:**

This project addressed the need for accurate and up-to-date information on EU State Aid grants within the Orbis platform. By automating the data extraction and validation process, this project improved the reliability and comprehensiveness of the data available to Orbis users, aiding in their decision-making processes.

**Contact:**

* LinkedIn: [URL](https://www.linkedin.com/in/kamalakarpeta/)

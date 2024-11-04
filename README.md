# Data Engineering Project: Redfin Data Pipeline

## Project Overview

This project is a comprehensive data engineering solution designed to fetch, process, and visualize real estate data from Redfin. The pipeline is built using a modern tech stack, including Python, Apache Airflow, Docker, Snowflake, and AWS Cloud S3. The primary goal is to automate the extraction, transformation, and loading (ETL) of Redfin data into Snowflake for further analysis and visualization using Power BI.

## Tech Stack

- **Python**: Core programming language for scripting and data manipulation.
- **Apache Airflow**: Workflow orchestration and management.
- **Docker**: Containerization of Airflow and other services.
- **Snowflake**: Cloud-based data warehousing for storing and querying data.
- **AWS S3**: Cloud storage for raw and transformed data.
- **Snowpipe**: Automatic data ingestion into Snowflake from S3.
- **Power BI**: Visualization and reporting.

## Project Workflow

1. **Data Extraction**: 
   - The pipeline fetches real estate data from Redfin's website.
   - The extracted data is stored as raw data in an S3 bucket.

2. **Data Transformation**:
   - Raw data is cleaned, structured, and transformed.
   - The transformed data is stored in a separate S3 bucket.

3. **Data Loading**:
   - The transformed data triggers Snowpipe, which automatically copies it into Snowflake tables.

4. **Data Visualization**:
   - Power BI connects to Snowflake to visualize the processed data for analysis and reporting.

## Project Architecture Diagram
![Redfin Image]((https://github.com/MLwithMuzammil/REDFIN-DATA-PIPELINE/blob/main/Redfin1.drawio.png))
## Setup and Installation

1. **Clone the Repository**
   ```bash
   git clone https://github.com/yourusername/redfin-data-pipeline.git
   cd redfin-data-pipeline
2. **Install all dependencies from requirements.txt**
3. **Pre requirements**
   Make sure you have linux platform to run apache airflow
   - you can either use dockers to run airflow webserver.
   - or a virtual machine with linux os installed.
   - or you can use ec2 instance of aws.
# REDFIN-DATA-PIPELINE

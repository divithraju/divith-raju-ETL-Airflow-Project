# Project Overview
This project demonstrates a simple ETL pipeline using Airflow, MySQL, Python, and Bash. The pipeline extracts data from a MySQL database, performs basic data transformation, and stores the result as a CSV file. The pipeline is scheduled and orchestrated using Apache Airflow.

# Key Features
1.Data Extraction: Retrieves sample data from a MySQL database.

2.Data Transformation: Filters records where the age is greater than 30.

3.Data Storage: Saves the transformed data as a CSV file in a specified directory.

4.Automation: The entire ETL process is automated using Airflow, with a DAG scheduled to run every 5 minutes.

# Project Structure

├── airflow_dag.py           # Defines the Airflow DAG and tasks

├── etl_script.py            # Python script containing the ETL process

├── wrapper_script.sh        # Bash script to run the Python ETL script

└── README.md                # Project documentation



# Prerequisites

Python 3.x

Apache Airflow

MySQL

Required Python Libraries: pandas, pymysql

# Usage
The ETL pipeline will automatically extract, transform, and load the data every 5 minutes as per the defined DAG schedule. The output CSV files will be stored in /home/ubuntu/extract.

# About
This project is designed to showcase a basic yet fully functional ETL pipeline using Airflow and Python. The pipeline handles real-world use cases like data extraction from MySQL, transformation based on conditions, and output storage as a CSV file. It also demonstrates how to integrate Python scripts with Airflow using Bash commands.




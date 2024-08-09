# Project Title: Spark SQL for Data Analysis (Home_Sales)

## Description:

This project demonstrates Spark SQL's capabilities for data analysis using a home sales dataset. It covers:

- Setting up a SparkSession in a Linux environment (replace with your specific setup instructions if necessary)
- Reading a CSV file from a URL (modify the URL with your actual data source)
- Creating and querying temporary views
- Performing basic data analysis tasks using Spark SQL syntax
- Exploring data caching for performance optimization
- Writing and reading data in Parquet format (a columnar file format)

## Requirements:

- A Linux environment with:
- Apache Spark (version 3.5.0 used in this example)
- Java (OpenJDK 11 used here)
- Python and pyspark library

## Instructions:

1. Install Dependencies:
apt-get update
apt-get install openjdk-11-jdk-headless -qq > /dev/null
wget -q https://archive.apache.org/dist/spark/spark-3.5.0/spark-3.5.0-bin-hadoop3-scala2.13.tgz
tar -xf spark-3.5.0-bin-hadoop3-scala2.13.tgz
pip install -q findspark

2. Set Environment Variables:
(Modify paths based on your actual installation locations)
     import os
os.environ["JAVA_HOME"] = "/usr/lib/jvm/java-11-openjdk-amd64"
os.environ["SPARK_HOME"] = '/content/spark-3.5.0-bin-hadoop3-scala2.13'

3. Run the Python Script:   

Execute the Python script (e.g., main.py) to perform data analysis tasks.

## Code Structure:

- The provided code snippet demonstrates:
- SparkSession creation
- CSV data loading with options (separator, header, etc.)
- Creating temporary views
- Sample queries for calculating average price based on various criteria
- Caching and uncaching temporary tables
- Writing and reading data in Parquet format
- You can adapt this structure to develop your own Spark SQL applications.

## Data Source:

- The code currently reads from a URL.
- Replace the URL with the actual location of your CSV data.

## Key Points:

- Spark SQL provides a powerful, scalable way to analyze large datasets.
- Temporary views create aliases for DataFrames, allowing for easier querying.
- Caching can significantly improve performance for repeated queries on the same data.
- Parquet format offers efficient storage and retrieval for columnar data.

## Further Exploration:

- Experiment with different Spark SQL functionalities for more complex data analysis tasks.
- Explore Spark's distributed processing capabilities for working with massive datasets.
- Consider integrating Spark with other frameworks like machine learning libraries.




# Stock-market-real-time-project-using-Kafka
Project Overview
This project implements a robust data engineering pipeline to simulate and process stock market data using Apache Kafka integrated with various AWS services. The architecture is designed to handle real-time data ingestion, processing, and querying, which is essential for financial applications requiring up-to-date information.

# Architecture
The pipeline comprises several components that work together to ensure efficient data flow from production to consumption:

# Data Production:

**SDK Boto3:** Utilized the AWS SDK for Python to interact with AWS services, facilitating operations such as data retrieval and storage.
Stock Market App Simulation: Simulated a stock market application to generate real-time financial data.
Dataset: The generated data is stored in a CSV format, making it easy to handle and transport.
Apache Kafka:

**Producer:** Configured a Kafka producer to publish the simulated stock market data onto a Kafka topic, ensuring reliable and consistent data flow.
Kafka Cluster: Managed the data across the Kafka cluster, providing a durable and scalable environment for data handling.
Consumer: Set up a Kafka consumer on an Amazon EC2 instance to subscribe to and process the data streamed through Kafka topics.
Data Storage and Processing:

**Amazon S3:** Integrated S3 to store the processed data, benefiting from its durability and scalability.
AWS Glue Crawler: Deployed a Glue Crawler to categorize and store metadata about the data in S3, enhancing data discoverability and accessibility.
AWS Glue Data Catalog: Utilized the data catalog as a centralized repository for metadata, which simplifies the management of data across disparate data storage systems.
Data Querying:

**Amazon Athena**: Enabled querying on the stored data using SQL with Amazon Athena, providing quick and efficient data analysis capabilities.

# Technologies Used
**Apache Kafka**: For real-time data streaming and handling.
**AWS Boto3**: For scripting AWS service interactions.
**Amazon S3**: For data storage.
**AWS Glue**: For data cataloging and search.
**Amazon Athena**: For executing SQL queries on data stored in S3.
**Amazon EC2**: For hosting Kafka consumers and other processing scripts.

# Setup and Configuration
Details about the setup and configuration can be included here, guiding how to configure Kafka, set up AWS services, and deploy the application.


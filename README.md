# Real-Time-Stock-Market-Kafka-DataEngineeringProject
## Introduction
In this project, I executed an end-to-end data engineering project focused on real-time stock market data using Apache Kafka. The project integrates various technologies such as Python, Amazon Web Services (AWS), Apache Kafka, Glue, Athena, and SQL to effectively handle, store, and analyze stock data.

## Architecture
The project architecture encompasses real-time data streaming, storage, and analysis through the following technologies:
## Architecture Diagram
<img src="Architecture.jpg">

## Technologies Used and Their Roles
### Programming Language - Python
I used Python to develop scripts that process and manage stock market data. Python interacts with Kafka to consume and produce real-time data streams.

### Amazon Web Services (AWS)

S3 (Simple Storage Service): I utilized S3 to securely store both raw and processed stock market data at scale. It serves as the primary storage solution for data ingested by Kafka.
Athena: I employed Athena for SQL-based analysis of the data stored in S3 without requiring a traditional database, allowing me to retrieve insights from the stock data efficiently.
Glue Crawler: I configured a Glue Crawler to automatically scan the data stored in S3 and create a metadata catalog, making it easier to query data with Athena.
Glue Catalog: I utilized the Glue Catalog to store metadata about the stock market data, enabling efficient querying and processing.
EC2: I leveraged EC2 to host and manage Kafka brokers and my Python applications, providing the necessary computing power to handle real-time data ingestion and processing.
### Apache Kafka
I implemented Kafka as the core technology for real-time data streaming. Kafka ingests live stock market data and distributes it across consumers for further processing, ensuring that stock data flows continuously and is readily available for near-instant analysis.

By integrating these technologies, I created a robust pipeline to collect, store, and analyze stock market data in real time, ensuring scalable and efficient performance throughout the project.

# Stock Market Real-Time Data Analysis Using Apache Kafka and AWS

## Project Overview
This project demonstrates a complete **end-to-end data engineering pipeline** for analyzing real-time stock market data using **Apache Kafka** and **Amazon Web Services (AWS)**. The goal is to build a scalable data pipeline capable of ingesting, processing, and analyzing stock market data in real time.

## Architecture

![Architecture](https://github.com/Prajwal0105/stock-market-real-time-data-analysis-using-kafka/blob/main/Architecture.jpg)

The architecture leverages **Apache Kafka** for data streaming and multiple AWS services, such as **S3**, **Glue**, **Athena**, and **EC2**, to store, process, and analyze the data.

---

## Technologies Used

- **Programming Language**: Python
- **Apache Kafka**: Real-time data streaming platform
- **Amazon Web Services (AWS)**:
  - **S3**: Data storage for raw and processed data
  - **Athena**: Querying and analyzing data using SQL
  - **Glue Crawler**: Crawls data in S3 to create metadata catalogs
  - **Glue Catalog**: Manages and stores metadata for Athena queries
  - **EC2**: Compute resources to run Apache Kafka and processing scripts

---

## Dataset Information
This project focuses on building the real-time data pipeline rather than analyzing a specific dataset. You can use any stock market data for real-time analysis, and for demonstration purposes, the following dataset is used:

**[Download Dataset](https://github.com/Prajwal0105/stock-market-real-time-data-analysis-using-kafka/blob/main/indexProcessed.csv)**

---

## Project Execution Flow

1. **Data Ingestion**:
   - Simulate stock market data using Python and stream it into a **Kafka cluster**.

2. **Data Processing**:
   - Consume the streamed data from Kafka and store it in **Amazon S3** as raw data.

3. **Crawling and Cataloging**:
   - Use **AWS Glue Crawler** to crawl the data in S3 and create a metadata catalog in **AWS Glue Catalog**.

4. **Data Analysis**:
   - Query the cataloged data using **Amazon Athena** and **SQL** for analysis.

---

## Installation & Setup

### 1. Clone the Repository

```bash
git clone https://github.com/Prajwal0105/stock-market-real-time-data-analysis-using-kafka.git
cd stock-market-real-time-data-analysis-using-kafka
```

### 2. Install Dependencies

Ensure you have **Python**, **Apache Kafka**, and necessary libraries installed:

```bash
pip install pandas kafka-python boto3
```

### 3. Set Up AWS

- Create an S3 bucket to store your data.
- Set up **AWS Glue** for the crawler and catalog.
- Use **Amazon EC2** for Kafka deployment and processing.

---

## Conclusion
This project demonstrates how to build and deploy a scalable **real-time data pipeline** for stock market analysis using **Apache Kafka** and **AWS services**. By integrating real-time data streaming with cloud-based storage and processing, this pipeline provides a robust solution for handling large-scale, continuous data flows.

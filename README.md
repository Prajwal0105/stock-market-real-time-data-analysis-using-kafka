# Stock Market Real-Time Data Analysis Using Kafka

## Description
In this project, we will execute an End-To-End Data Engineering Project on Real-Time Stock Market Data using Kafka. We are using different technologies such as Python, Amazon Web Services (AWS), Apache Kafka, Glue, Athena, and SQL

## Architecture
![Architecture](https://github.com/Prajwal0105/stock-market-real-time-data-analysis-using-kafka/blob/main/Architecture.jpg)

## Technology Used
- Programming Language - Python
- Apache Kafka
- Amazon Web Service (AWS)
  - S3 (Simple Storage Service)
  - Athena
  - Glue Crawler
  - Glue Catalog
  - EC2
 
## Dataset Used
We can use any dataset, in this project it is mainly in operation side of Data Engineering (building data pipeline)

Here is the dataset used - [Dataset file](https://github.com/Prajwal0105/stock-market-real-time-data-analysis-using-kafka/blob/main/indexProcessed.csv)

## Project Execution flow
- Take some stock market data
- Use python to produce that data and put in Kafka clusture
- Then we will consume that data and store it in Amazon S3
- Crawl this data using Crawler to build a Glue catalog
- Analyze the data using Amazon Athena using SQL

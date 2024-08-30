# YouTube Data Analysis Project by Shashank Pandey

## Overview

This project aims to securely manage, streamline, and perform analysis on structured and semi-structured YouTube videos data based on video categories and trending metrics. We'll be using various AWS services to create a scalable, cloud-based solution for data ingestion, processing, and analysis.

## Project Goals

1. **Data Ingestion**: Build a mechanism to ingest data from different sources.
2. **ETL System**: Transform raw data into the proper format for analysis.
3. **Data Lake**: Create a centralized repository to store data from multiple sources.
4. **Scalability**: Ensure the system scales as the size of our data increases.
5. **Cloud Infrastructure**: Utilize AWS services to process vast amounts of data.
6. **Reporting**: Build a dashboard to visualize data and answer key questions.

## AWS Services Used

- **Amazon S3**: Object storage service for scalable data storage.
- **AWS IAM**: Identity and Access Management for secure access control.
- **Amazon QuickSight**: Scalable, serverless business intelligence (BI) service for data visualization.
- **AWS Glue**: Serverless data integration service for data discovery, preparation, and combination.
- **AWS Lambda**: Serverless computing service for running code without managing servers.
- **AWS Athena**: Interactive query service for S3 data.

## Dataset

We're using a Kaggle dataset containing statistics on daily popular YouTube videos over several months. The dataset includes:

- Up to 200 trending videos published daily for various locations.
- Data for each region in separate files.
- Video information such as title, channel title, publication time, tags, views, likes, dislikes, description, and comment count.
- A `category_id` field (varies by region) included in a linked JSON file.

Dataset source: [YouTube Trending Video Dataset](https://www.kaggle.com/datasets/datasnaek/youtube-new)

## Project Structure

1. Clone the repository to your local machine.
2. Set up your AWS credentials and configure the necessary IAM roles and permissions.
3. Ingest data from the Kaggle dataset into Amazon S3.
4. Use AWS Glue to transform and load data into the data lake.
5. Query the data with AWS Athena and visualize results with Amazon QuickSight.
6. Deploy your Lambda functions to automate the process and ensure scalability.
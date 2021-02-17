# Data Warehose with AWS Redshift project for Udacity Data Engineer Nanodegree

## Project overview
This is Data Warehouse project for Udacity Data Engineer Nanodegree. In this project I create an **ETL pipeline** that extracts data from **AWS S3** and loads it into a database schema using **AWS Redshift** as staging mechanism.  This JSON files represent a user activity logs collected by a music streaming app of an imaginary startup Sparkify. And the resulting database will be used for analytical purposes.

## Python scripts
* create_tables.py: Drop previous schema and creates empty tables
* sql_queries.py: Defines all queries used in the ETL pipeline
* etl.py: Loads data from the JSON files into the tables

## Database schema

### Fact Table:
* songplays: Records of song plays in log files 

### Dimension Tables:
* artists: Artists in the music database
* songs: Songs in the music database
* users: Users of the app
* time: Timestamps of records

### Staging tables for ETL:
* staging_events: Event data telling what users have done 
* staging_songs: Song data about songs and artists 

## Prerequisites
The code is **Python** scripts and it requires:

* [AWS Account](https://aws.amazon.com/)
* [Psycopg](https://pypi.org/project/psycopg2/)

## Run the Code

`python create_tables.py`
`python etl.py`


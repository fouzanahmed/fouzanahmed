# Fouzan Ahmed

Data engineer in Melbourne. I build the pipeline, the warehouse and the dashboard that sits on top, and I care most about the part where it keeps running after I stop watching it.

My best debugging story so far is from Principal Financial. A Morningstar ingestion job had been failing in one environment for months and nobody could reproduce it anywhere else. An S3 listing call was not paginated, so it silently stopped at 1,000 objects, and only the environment with the biggest file backlog ever crossed that line. One line to fix. A long time to find.

Right now I am building an APRA superannuation analytics platform end to end, from Airflow ingestion through dbt marts to a live Power BI dashboard, plus a natural language to SQL layer on top.

## Projects

| Project | What it does | Stack |
|---|---|---|
| [APRA Superannuation Analytics Platform](https://github.com/fouzanahmed/apra-super-pipeline) | Weekly pipeline over APRA regulatory filings, landing raw files in S3, upserting into RDS Postgres, running dbt marts, and serving a live Power BI dashboard. Includes a FastAPI endpoint that turns plain English questions into SQL. | Airflow, dbt, AWS, PostgreSQL, Docker, FastAPI, Power BI |
| Market Data Warehouse on Snowflake | Three-layer warehouse over five years of daily prices for 1,000 tickers. Streams and tasks drive the daily MERGE, Time Travel snapshots keep lookahead bias out of backtesting, and a clustering key fixed some ugly partition scans. | Snowflake, SQL, Python, S3 |
| StreamPredict | Real-time food delivery time prediction. Kafka produces the orders, Spark Structured Streaming consumes them, and a PySpark MLlib model scores each one as it arrives. | Kafka, PySpark, Spark Structured Streaming, MLlib |
| [eSafety Threat Detection](https://github.com/fouzanahmed/ESafety-Threat-Detection) | Multi-modal content safety platform built at a hackathon. Scores social media posts across eight harm categories using GPT-4 and Gemini, and pulls video frames with FFmpeg so it reads more than just text. | Node.js, React, TypeScript, GPT-4, Gemini, Docker |
| BirdTag | Serverless AWS app that detects and tags bird species in uploaded images, audio and video. S3 upload events fan out to Lambdas for inference, thumbnails and indexing. | Lambda, S3, API Gateway, DynamoDB, Cognito, OpenCV |

## Stack

**Data** Python, SQL, pandas, PySpark, dbt, Airflow, Kafka
**Warehouses and databases** Snowflake, PostgreSQL, DynamoDB
**Cloud** AWS (Lambda, S3, EC2, RDS, Glue, CDK, CloudWatch), Docker, GitHub Actions
**BI** Power BI, DAX, Tableau
**Other** FastAPI, LangChain, RAG, React

## Elsewhere

[LinkedIn](https://www.linkedin.com/in/fouzanfahmed) · fouzanf.ahmed@gmail.com

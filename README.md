<h1 align="center">Fouzan Ahmed</h1>

<p align="center">Data Engineer &nbsp;·&nbsp; Melbourne, Australia</p>

<p align="center">
  <a href="https://www.linkedin.com/in/fouzanfahmed"><img src="https://img.shields.io/badge/LinkedIn-1F2328?style=flat-square&logo=linkedin&logoColor=white" alt="LinkedIn"/></a>
  <a href="mailto:fouzanf.ahmed@gmail.com"><img src="https://img.shields.io/badge/Email-1F2328?style=flat-square&logo=gmail&logoColor=white" alt="Email"/></a>
</p>

---

### About

I build the pipeline, the warehouse and the dashboard that sits on top, and I care most about the part where it keeps running after I stop watching it.

My best debugging story so far is from Principal Financial. A Morningstar ingestion job had been failing in one environment for months and nobody could reproduce it anywhere else. An S3 listing call was not paginated, so it silently stopped at 1,000 objects, and only the environment with the biggest file backlog ever crossed that line. One line to fix. A long time to find.

Currently building an APRA superannuation analytics platform end to end, from Airflow ingestion through dbt marts to a live Power BI dashboard, with a natural language to SQL layer on top.

---

### Tech Stack

**Languages and frameworks**

<p>
  <img src="https://img.shields.io/badge/Python-1F2328?style=flat-square&logo=python&logoColor=white"/>
  <img src="https://img.shields.io/badge/SQL-1F2328?style=flat-square&logo=postgresql&logoColor=white"/>
  <img src="https://img.shields.io/badge/pandas-1F2328?style=flat-square&logo=pandas&logoColor=white"/>
  <img src="https://img.shields.io/badge/PySpark-1F2328?style=flat-square&logo=apachespark&logoColor=white"/>
  <img src="https://img.shields.io/badge/Airflow-1F2328?style=flat-square&logo=apacheairflow&logoColor=white"/>
  <img src="https://img.shields.io/badge/dbt-1F2328?style=flat-square&logo=dbt&logoColor=white"/>
  <img src="https://img.shields.io/badge/Kafka-1F2328?style=flat-square&logo=apachekafka&logoColor=white"/>
  <img src="https://img.shields.io/badge/FastAPI-1F2328?style=flat-square&logo=fastapi&logoColor=white"/>
  <img src="https://img.shields.io/badge/React-1F2328?style=flat-square&logo=react&logoColor=white"/>
  <img src="https://img.shields.io/badge/TypeScript-1F2328?style=flat-square&logo=typescript&logoColor=white"/>
</p>

**Cloud and infrastructure**

<p>
  <img src="https://img.shields.io/badge/AWS-1F2328?style=flat-square&logo=amazonwebservices&logoColor=white"/>
  <img src="https://img.shields.io/badge/Lambda-1F2328?style=flat-square&logo=awslambda&logoColor=white"/>
  <img src="https://img.shields.io/badge/S3-1F2328?style=flat-square&logo=amazons3&logoColor=white"/>
  <img src="https://img.shields.io/badge/Azure-1F2328?style=flat-square&logo=microsoftazure&logoColor=white"/>
  <img src="https://img.shields.io/badge/Docker-1F2328?style=flat-square&logo=docker&logoColor=white"/>
  <img src="https://img.shields.io/badge/GitHub%20Actions-1F2328?style=flat-square&logo=githubactions&logoColor=white"/>
  <img src="https://img.shields.io/badge/Git-1F2328?style=flat-square&logo=git&logoColor=white"/>
  <img src="https://img.shields.io/badge/Linux-1F2328?style=flat-square&logo=linux&logoColor=white"/>
</p>

**Databases and warehousing**

<p>
  <img src="https://img.shields.io/badge/Snowflake-1F2328?style=flat-square&logo=snowflake&logoColor=white"/>
  <img src="https://img.shields.io/badge/PostgreSQL-1F2328?style=flat-square&logo=postgresql&logoColor=white"/>
  <img src="https://img.shields.io/badge/DynamoDB-1F2328?style=flat-square&logo=amazondynamodb&logoColor=white"/>
  <img src="https://img.shields.io/badge/MongoDB-1F2328?style=flat-square&logo=mongodb&logoColor=white"/>
</p>

**Analytics and AI**

<p>
  <img src="https://img.shields.io/badge/Power%20BI-1F2328?style=flat-square&logo=powerbi&logoColor=white"/>
  <img src="https://img.shields.io/badge/Tableau-1F2328?style=flat-square&logo=tableau&logoColor=white"/>
  <img src="https://img.shields.io/badge/LangChain-1F2328?style=flat-square&logo=langchain&logoColor=white"/>
  <img src="https://img.shields.io/badge/OpenAI-1F2328?style=flat-square&logo=openai&logoColor=white"/>
  <img src="https://img.shields.io/badge/n8n-1F2328?style=flat-square&logo=n8n&logoColor=white"/>
</p>

---

### Projects

| Project | What it does | Stack |
|---|---|---|
| [**APRA Superannuation Analytics Platform**](https://github.com/fouzanahmed/apra-super-pipeline) | Weekly pipeline over APRA regulatory filings, landing raw files in S3, upserting into RDS Postgres, running dbt marts, and serving a live Power BI dashboard. Includes a FastAPI endpoint that turns plain English questions into SQL. | Airflow, dbt, AWS, PostgreSQL, Docker, FastAPI, Power BI |
| **Market Data Warehouse on Snowflake** | Three-layer warehouse over five years of daily prices for 1,000 tickers. Streams and tasks drive the daily MERGE, Time Travel snapshots keep lookahead bias out of backtesting, and a clustering key fixed some ugly partition scans. | Snowflake, SQL, Python, S3 |
| **StreamPredict** | Real-time food delivery time prediction. Kafka produces the orders, Spark Structured Streaming consumes them, and a PySpark MLlib model scores each one as it arrives. | Kafka, PySpark, Structured Streaming, MLlib |
| [**eSafety Threat Detection**](https://github.com/fouzanahmed/ESafety-Threat-Detection) | Multi-modal content safety platform built at a hackathon. Scores social media posts across eight harm categories using GPT-4 and Gemini, and pulls video frames with FFmpeg so it reads more than just text. | Node.js, React, TypeScript, GPT-4, Gemini, Docker |
| **BirdTag** | Serverless AWS app that detects and tags bird species in uploaded images, audio and video. S3 upload events fan out to Lambdas for inference, thumbnails and indexing. | Lambda, S3, API Gateway, DynamoDB, Cognito, OpenCV |

---

### Contributions

<picture>
  <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/fouzanahmed/fouzanahmed/output/github-snake-dark.svg" />
  <source media="(prefers-color-scheme: light)" srcset="https://raw.githubusercontent.com/fouzanahmed/fouzanahmed/output/github-snake.svg" />
  <img alt="contribution graph animation" src="https://raw.githubusercontent.com/fouzanahmed/fouzanahmed/output/github-snake.svg" />
</picture>

---

### Certifications

AWS Certified Developer Associate &nbsp;·&nbsp; Snowflake SnowPro Core &nbsp;·&nbsp; Microsoft Power BI Data Analyst (PL-300) &nbsp;·&nbsp; Azure Fundamentals (AZ-900)

---

### Outside work

Cricket, chess, and teaching kids to code.

<p align="center"><i>Open to data engineering roles across Australia.</i></p>

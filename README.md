<h1 align="center">Fouzan Ahmed</h1>

<p align="center">Data Engineer &amp; Analyst &nbsp;·&nbsp; Australia</p>

<p align="center">
  <a href="https://fouzanahmed.vercel.app"><img src="https://img.shields.io/badge/Website-1F2328?style=flat-square&logo=vercel&logoColor=white" alt="Website"/></a>
  <a href="https://www.linkedin.com/in/fouzanf-ahmed/"><img src="https://img.shields.io/badge/LinkedIn-1F2328?style=flat-square&logo=linkedin&logoColor=white" alt="LinkedIn"/></a>
  <a href="mailto:fouzanf.ahmed@gmail.com"><img src="https://img.shields.io/badge/Email-1F2328?style=flat-square&logo=gmail&logoColor=white" alt="Email"/></a>
</p>

---

### About

I build the pipeline, the warehouse and the dashboard that sits on top, and I care most about the part where it keeps running after I stop watching it.

My best debugging story so far is from Principal Financial. A Morningstar ingestion job had been failing in one environment for months and nobody could reproduce it anywhere else. An S3 listing call was not paginated, so it silently stopped at 1,000 objects, and only the environment with the biggest file backlog ever crossed that line. I cleared the backlog to unblock the release that day, then added pagination so it couldn't come back.

These days I'm a Data Analyst at UMNT, a community organization in Darwin, where I built their first data pipeline and Power BI dashboards from scratch. On the side I'm hardening an APRA superannuation pipeline with a Claude text-to-SQL layer, and running pruning and cost experiments on a Snowflake warehouse.

> *"He went from being new to the team to someone I could confidently trust with meaningful work."*
> Rahul Yadav, my mentor at Principal ([more on my site](https://fouzanahmed.vercel.app/#recommendations))

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
  <img src="https://img.shields.io/badge/Claude%20API-1F2328?style=flat-square&logo=claude&logoColor=white"/>
  <img src="https://img.shields.io/badge/Hugging%20Face-1F2328?style=flat-square&logo=huggingface&logoColor=white"/>
  <img src="https://img.shields.io/badge/PyTorch-1F2328?style=flat-square&logo=pytorch&logoColor=white"/>
  <img src="https://img.shields.io/badge/n8n-1F2328?style=flat-square&logo=n8n&logoColor=white"/>
</p>

---

### Projects

| Project | What it does | Stack |
|---|---|---|
| [**APRA Superannuation Analytics Platform**](https://github.com/fouzanahmed/apra-super-pipeline) | Weekly Airflow pipeline over APRA's quarterly MySuper filings. Raw runs are archived in S3 and replayable, dbt models it with 21 passing tests, and a FastAPI endpoint lets Claude turn plain-English questions into SQL inside a read-only transaction. Found a silent join that left fund assets 100% NULL and took matched rows from 0 to 589. | Airflow, dbt, AWS, PostgreSQL, Claude API, Docker |
| [**Market Data Warehouse on Snowflake**](https://github.com/fouzanahmed/snowflake-market-warehouse) | Layered warehouse over 11 years of daily prices for 501 S&P 500 tickers. 1,338,849 rows load in 2.4 seconds, a stream and task drive the daily MERGE, and a CTAS re-sort cut a query from 8 of 8 partitions to 2 of 8 without paying for a clustering key. | Snowflake, SQL, Python |
| [**StreamPredict**](https://github.com/fouzanahmed/streampredict) | Monash coursework (FIT5202), so some files are kept private. Real-time food delivery time prediction. Kafka produces the orders, Spark Structured Streaming consumes them, and a PySpark MLlib model scores each one as it arrives. Gradient boosted trees took RMSE from 7.79 to 3.10, and tuning brought it to 2.979. | Kafka, PySpark, Structured Streaming, MLlib |
| [**eSafety Threat Detection**](https://github.com/fouzanahmed/ESafety-Threat-Detection) | Multi-modal content safety platform built at a hackathon. Scores social media posts across eight harm categories using GPT-4 and Gemini, and pulls video frames with FFmpeg so it reads more than just text. | Node.js, React, TypeScript, GPT-4, Gemini, FFmpeg |
| **BirdTag** | Serverless AWS app that detects and tags bird species in uploaded images, audio and video. S3 upload events fan out to Lambdas for inference, thumbnails and indexing. | Lambda, S3, API Gateway, DynamoDB, Cognito, OpenCV |
| **eSafety Kaggle Classifier** | 3rd place on the eSafety Hackathon Kaggle leaderboard. Fine-tuned DeBERTa-v3-large across 13 harmful-content categories, with focal loss and a tuned threshold per label. | PyTorch, Hugging Face, DeBERTa |
| **Weather, Together** | Suburb-level flood, bushfire and heat risk for Melbourne, combining 130+ years of SILO climate records, live BOM feeds and fire danger projections behind a FastAPI and PostGIS backend. Voted best project in the Environment theme. | FastAPI, PostgreSQL, PostGIS, Mapbox, QGIS |
| [**NewsFlow**](https://github.com/fouzanahmed/newsflow) | AI news digest, built with a teammate, delivered to Telegram at 9 AM every day, plus an n8n agent that turns the news into a newsletter and narrated video. | n8n, LangGraph, Claude API, SQLite |

---

### Contributions

<picture>
  <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/fouzanahmed/fouzanahmed/output/github-snake-dark.svg" />
  <source media="(prefers-color-scheme: light)" srcset="https://raw.githubusercontent.com/fouzanahmed/fouzanahmed/output/github-snake.svg" />
  <img alt="contribution graph animation" src="https://raw.githubusercontent.com/fouzanahmed/fouzanahmed/output/github-snake.svg" />
</picture>

---

### Certifications

[Snowflake SnowPro Core](https://achieve.snowflake.com/01a9f515-65ae-4c45-ac9b-663b8b5feeaa#acc.gfk7BrMJ) &nbsp;·&nbsp; [AWS Certified AI Practitioner](https://www.credly.com/badges/109a51f2-7525-47d6-9de2-7cabdd5c6939/public_url) &nbsp;·&nbsp; [Azure Data Fundamentals (DP-900)](https://learn.microsoft.com/en-us/users/fouzanahmed-2192/transcript/d88mbremnyxkzjd) &nbsp;·&nbsp; AWS Certified Developer Associate &nbsp;·&nbsp; dbt Analytics Engineering &nbsp;·&nbsp; Power BI Data Analyst (PL-300)

[All 11 on my site](https://fouzanahmed.vercel.app/#certifications)

---

### Outside work

Cricket, chess, and teaching kids to code.

<p align="center"><i>Open to data engineering and data analyst roles across Australia.</i></p>

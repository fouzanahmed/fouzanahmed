<h1 align="center">Hi, I'm Fouzan 👋</h1>

<p align="center">
  <a href="https://www.linkedin.com/in/fouzanfahmed"><img src="https://img.shields.io/badge/LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white" alt="LinkedIn"/></a>
  <a href="mailto:fouzanf.ahmed@gmail.com"><img src="https://img.shields.io/badge/Email-EA4335?style=for-the-badge&logo=gmail&logoColor=white" alt="Email"/></a>
  <img src="https://komarev.com/ghpvc/?username=fouzanahmed&style=for-the-badge&color=blue" alt="Profile views"/>
</p>

---

### 🧑‍💻 About

Data engineer in Melbourne. I build the pipeline, the warehouse and the dashboard that sits on top, and I care most about the part where it keeps running after I stop watching it.

My best debugging story so far is from Principal Financial. A Morningstar ingestion job had been failing in one environment for months and nobody could reproduce it anywhere else. An S3 listing call was not paginated, so it silently stopped at 1,000 objects, and only the environment with the biggest file backlog ever crossed that line. One line to fix. A long time to find.

- 🔭 Currently building an **APRA superannuation analytics platform**, Airflow to dbt to Power BI, with a natural language to SQL layer on top
- 🌱 Learning more about **agentic workflows** and where LLMs actually earn their place in a data stack
- 💬 Ask me about Snowflake warehouse design, Airflow DAGs, or why your Lambda keeps timing out
- 📫 Reach me at **fouzanf.ahmed@gmail.com**

---

## 💻 Tech Stack

**🛠️ Languages & Frameworks**

![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)
![SQL](https://img.shields.io/badge/SQL-025E8C?style=for-the-badge&logo=database&logoColor=white)
![Pandas](https://img.shields.io/badge/pandas-150458?style=for-the-badge&logo=pandas&logoColor=white)
![PySpark](https://img.shields.io/badge/Apache%20Spark-E25A1C?style=for-the-badge&logo=apachespark&logoColor=white)
![Airflow](https://img.shields.io/badge/Airflow-017CEE?style=for-the-badge&logo=apacheairflow&logoColor=white)
![dbt](https://img.shields.io/badge/dbt-FF694B?style=for-the-badge&logo=dbt&logoColor=white)
![Kafka](https://img.shields.io/badge/Kafka-231F20?style=for-the-badge&logo=apachekafka&logoColor=white)
![FastAPI](https://img.shields.io/badge/FastAPI-009688?style=for-the-badge&logo=fastapi&logoColor=white)
![React](https://img.shields.io/badge/React-20232A?style=for-the-badge&logo=react&logoColor=61DAFB)
![TypeScript](https://img.shields.io/badge/TypeScript-3178C6?style=for-the-badge&logo=typescript&logoColor=white)

**☁️ Cloud & DevOps**

![AWS](https://img.shields.io/badge/AWS-232F3E?style=for-the-badge&logo=amazonwebservices&logoColor=white)
![Lambda](https://img.shields.io/badge/Lambda-FF9900?style=for-the-badge&logo=awslambda&logoColor=white)
![S3](https://img.shields.io/badge/S3-569A31?style=for-the-badge&logo=amazons3&logoColor=white)
![Azure](https://img.shields.io/badge/Azure-0078D4?style=for-the-badge&logo=microsoftazure&logoColor=white)
![Docker](https://img.shields.io/badge/Docker-2496ED?style=for-the-badge&logo=docker&logoColor=white)
![GitHub Actions](https://img.shields.io/badge/GitHub%20Actions-2088FF?style=for-the-badge&logo=githubactions&logoColor=white)
![Git](https://img.shields.io/badge/Git-F05032?style=for-the-badge&logo=git&logoColor=white)
![Linux](https://img.shields.io/badge/Linux-FCC624?style=for-the-badge&logo=linux&logoColor=black)

**🗃️ Databases & Warehousing**

![Snowflake](https://img.shields.io/badge/Snowflake-29B5E8?style=for-the-badge&logo=snowflake&logoColor=white)
![PostgreSQL](https://img.shields.io/badge/PostgreSQL-4169E1?style=for-the-badge&logo=postgresql&logoColor=white)
![DynamoDB](https://img.shields.io/badge/DynamoDB-4053D6?style=for-the-badge&logo=amazondynamodb&logoColor=white)
![MongoDB](https://img.shields.io/badge/MongoDB-47A248?style=for-the-badge&logo=mongodb&logoColor=white)

**📊 BI & AI**

![Power BI](https://img.shields.io/badge/Power%20BI-F2C811?style=for-the-badge&logo=powerbi&logoColor=black)
![Tableau](https://img.shields.io/badge/Tableau-E97627?style=for-the-badge&logo=tableau&logoColor=white)
![LangChain](https://img.shields.io/badge/LangChain-1C3C3C?style=for-the-badge&logo=langchain&logoColor=white)
![OpenAI](https://img.shields.io/badge/OpenAI-412991?style=for-the-badge&logo=openai&logoColor=white)
![n8n](https://img.shields.io/badge/n8n-EA4B71?style=for-the-badge&logo=n8n&logoColor=white)

---

## 🚀 Projects

| Project | What it does | Stack |
|---|---|---|
| [**APRA Superannuation Analytics Platform**](https://github.com/fouzanahmed/apra-super-pipeline) | Weekly pipeline over APRA regulatory filings, landing raw files in S3, upserting into RDS Postgres, running dbt marts, and serving a live Power BI dashboard. Includes a FastAPI endpoint that turns plain English questions into SQL. | Airflow, dbt, AWS, PostgreSQL, Docker, FastAPI, Power BI |
| **Market Data Warehouse on Snowflake** | Three-layer warehouse over five years of daily prices for 1,000 tickers. Streams and tasks drive the daily MERGE, Time Travel snapshots keep lookahead bias out of backtesting, and a clustering key fixed some ugly partition scans. | Snowflake, SQL, Python, S3 |
| **StreamPredict** | Real-time food delivery time prediction. Kafka produces the orders, Spark Structured Streaming consumes them, and a PySpark MLlib model scores each one as it arrives. | Kafka, PySpark, Structured Streaming, MLlib |
| [**eSafety Threat Detection**](https://github.com/fouzanahmed/ESafety-Threat-Detection) | Multi-modal content safety platform built at a hackathon. Scores social media posts across eight harm categories using GPT-4 and Gemini, and pulls video frames with FFmpeg so it reads more than just text. | Node.js, React, TypeScript, GPT-4, Gemini, Docker |
| **BirdTag** | Serverless AWS app that detects and tags bird species in uploaded images, audio and video. S3 upload events fan out to Lambdas for inference, thumbnails and indexing. | Lambda, S3, API Gateway, DynamoDB, Cognito, OpenCV |

---

## 🐍 Contribution Snake

<picture>
  <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/fouzanahmed/fouzanahmed/output/github-snake-dark.svg" />
  <source media="(prefers-color-scheme: light)" srcset="https://raw.githubusercontent.com/fouzanahmed/fouzanahmed/output/github-snake.svg" />
  <img alt="github contribution grid snake animation" src="https://raw.githubusercontent.com/fouzanahmed/fouzanahmed/output/github-snake.svg" />
</picture>

---

## 📈 Stats

<p align="center">
  <img height="165" src="https://github-readme-stats.vercel.app/api?username=fouzanahmed&show_icons=true&theme=tokyonight&hide_border=true&count_private=true" alt="stats"/>
  <img height="165" src="https://github-readme-stats.vercel.app/api/top-langs/?username=fouzanahmed&layout=compact&theme=tokyonight&hide_border=true&langs_count=8&hide=html,css" alt="top languages"/>
</p>

---

## 🎮 Beyond the Terminal

🏏 Cricket, badly but enthusiastically &nbsp;•&nbsp; ♟️ Chess and puzzles &nbsp;•&nbsp; 📚 Reading &nbsp;•&nbsp; 🎮 Games &nbsp;•&nbsp; 🧑‍🏫 Teaching kids to code

---

<p align="center"><i>Open to data engineering roles across Australia.</i></p>

\# 🚀 2.5M Reviews — Streaming Sentiment Intelligence



An end-to-end Data Engineering and Analytics project built using \*\*Databricks, PySpark, Delta Lake, SQL, Structured Streaming, and Power BI\*\*.



The project processes approximately \*\*2.5 million review records\*\* through a \*\*Medallion Architecture\*\* and transforms raw review data into business-ready sentiment and engagement analytics.



\---



\## 📌 Project Overview



This project demonstrates a complete data pipeline from raw review ingestion to business intelligence reporting.



\### Pipeline



```text

2.5M Reviews Dataset

&#x20;       ↓

Databricks Volume

&#x20;       ↓

Bronze Layer

&#x20;       ↓

Silver Layer

&#x20;       ↓

Gold Layer

&#x20;       ↓

SQL Analytics

&#x20;       ↓

Power BI Dashboard

````



\---



\## 🏗️ Architecture



```text

&#x20;                   2.5M Reviews Dataset

&#x20;                           │

&#x20;                           ▼

&#x20;                   Databricks Volume

&#x20;                           │

&#x20;                           ▼

&#x20;                   ┌───────────────┐

&#x20;                   │    BRONZE     │

&#x20;                   │   Raw Data    │

&#x20;                   │  Delta Table  │

&#x20;                   └───────┬───────┘

&#x20;                           │

&#x20;                           ▼

&#x20;                   ┌───────────────┐

&#x20;                   │    SILVER     │

&#x20;                   │   Cleaning    │

&#x20;                   │  Validation   │

&#x20;                   │ NLP Features  │

&#x20;                   └───────┬───────┘

&#x20;                           │

&#x20;                           ▼

&#x20;                   ┌───────────────┐

&#x20;                   │     GOLD      │

&#x20;                   │ Aggregations  │

&#x20;                   │ Business KPIs │

&#x20;                   └───────┬───────┘

&#x20;                           │

&#x20;                  ┌────────┴────────┐

&#x20;                  ▼                 ▼

&#x20;             SQL Analytics      Power BI

&#x20;                  │                 │

&#x20;                  └────────┬────────┘

&#x20;                           ▼

&#x20;                 Sentiment Intelligence

&#x20;                      Dashboard

```



\---



\## 🛠️ Technologies Used



| Technology           | Purpose                     |

| -------------------- | --------------------------- |

| Python               | Data processing             |

| PySpark              | Distributed data processing |

| Databricks           | Data Engineering            |

| Delta Lake           | Data storage                |

| SQL                  | Data analytics              |

| Structured Streaming | Streaming pipeline          |

| Power BI             | Dashboard and visualization |

| Git/GitHub           | Version control             |



\---



\## 🥉 Bronze Layer



The Bronze layer stores the raw review data.



\### Operations



\* Raw data ingestion

\* Schema handling

\* Initial data loading

\* Delta table creation

\* Raw data preservation



\### Notebook



`databricks/01\_Data\_Ingestion\_Bronze.ipynb`



\---



\## 🥈 Silver Layer



The Silver layer performs data cleaning, validation, and feature engineering.



\### Transformations



\* Column standardization

\* Null handling

\* Data type conversion

\* Timestamp processing

\* Text cleaning

\* Duplicate removal

\* Data validation

\* Sentiment standardization



\### Feature Engineering



The pipeline creates analytical text and engagement features such as:



\* Text length

\* Word count

\* Character count

\* Engagement-related metrics



\### Notebook



`databricks/02\_silver\_transformation.ipynb`



\---



\## 🥇 Gold Layer



The Gold layer contains business-ready analytical datasets.



\### Analysis



\* Sentiment distribution

\* Platform analysis

\* Country analysis

\* Engagement analysis

\* Time-based analysis

\* Sentiment trends



\### Notebook



`databricks/03\_Gold\_Analytics.ipynb`



\---



\## 🔎 SQL Analytics



SQL is used to analyze the processed data.



\### Analysis Includes



\* Total review count

\* Sentiment distribution

\* Reviews by platform

\* Reviews by country

\* Engagement analysis

\* Sentiment by platform

\* Time-based analysis

\* Review trends



\### Notebook



`databricks/04\_SQL\_Analysis.ipynb`



\---



\## ⚡ Streaming Pipeline



A Structured Streaming pipeline is included for incremental processing.



\### Streaming Flow



```text

Incoming Review Files

&#x20;       ↓

Auto Loader

&#x20;       ↓

Streaming Bronze

&#x20;       ↓

Streaming Silver

&#x20;       ↓

Streaming Gold

&#x20;       ↓

Analytics

```



\### Concepts Demonstrated



\* Incremental ingestion

\* Structured Streaming

\* Delta Lake

\* Checkpointing

\* Continuous data processing



\### Notebook



`databricks/05\_Streaming\_Pipeline.ipynb`



\---



\## 📊 Power BI Dashboard



A \*\*one-page Power BI dashboard\*\* provides a business view of sentiment and engagement.



\### KPIs



\* Total Reviews

\* Average Engagement

\* Average Likes

\* Average Retweets

\* Average Words per Review



\### Visualizations



\* Sentiment Distribution

\* Reviews by Platform

\* Average Engagement by Platform

\* Sentiment by Platform

\* Top 10 Countries by Reviews

\* Sentiment Trend Over Time

\* Hourly Sentiment Activity



\### Power BI File



`powerbi/Streaming\_Sentiment\_Intelligence.pbix`



\### Power BI Notebook



`databricks/06\_PowerBI\_Export.ipynb`



\---



\## 📸 Dashboard Preview



!\[Streaming Sentiment Intelligence Dashboard](screenshots/sentiment\_dashboard.png)



\---



\## 📁 Project Structure



```text

2.5M-Reviews-Streaming-Sentiment-Intelligence/

│

├── databricks/

│   ├── 01\_Data\_Ingestion\_Bronze.ipynb

│   ├── 02\_silver\_transformation.ipynb

│   ├── 03\_Gold\_Analytics.ipynb

│   ├── 04\_SQL\_Analysis.ipynb

│   ├── 05\_Streaming\_Pipeline.ipynb

│   └── 06\_PowerBI\_Export.ipynb

│

├── powerbi/

│   └── Streaming\_Sentiment\_Intelligence.pbix

│

├── screenshots/

│   └── sentiment\_dashboard.png

│

├── README.md

│

└── .gitignore

```



\---



\## 🎯 Business Questions



The project helps answer:



1\. What is the overall sentiment distribution?

2\. Which platforms have the highest review volume?

3\. Which platforms generate higher engagement?

4\. Which countries contribute the most reviews?

5\. How does sentiment vary across platforms?

6\. How does sentiment change over time?

7\. During which hours is review activity highest?

8\. Which sentiment categories receive the most engagement?



\---



\## 📈 Key Skills Demonstrated



\### Data Engineering



\* Databricks

\* ETL/ELT

\* Medallion Architecture

\* Delta Lake

\* PySpark

\* Structured Streaming

\* Batch Processing

\* Data Cleaning

\* Data Quality

\* Data Transformation



\### Data Analytics

\* SQL

\* PySpark

\* Sentiment Analysis

\* Engagement Analysis

\* Time-Series Analysis

\* KPI Development

\* Business Intelligence





\---



\## 🚀 Future Improvements



\* Real-time ML-based sentiment classification

\* Kafka integration

\* MLflow model tracking

\* Databricks Workflows automation

\* Real-time Power BI refresh

\* Advanced NLP models

\* Automated data quality monitoring



\---



\## 👩‍💻 Author



\*\*Gauri Sutar\*\*



Data Analyst | Data Engineer | Data Science \& ML Enthusiast



```




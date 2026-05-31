# Hi, I'm Ansu John 👋

**Senior Data Engineer** with hands-on experience designing production-grade data pipelines, real-time streaming architectures, AI-augmented data platforms, and cloud-native data warehousing solutions. I build end-to-end systems — from raw ingestion to analytical marts — with a focus on reliability, observability, and modern data stack best practices.

📍 Kochi, India &nbsp;|&nbsp; 🔗 [LinkedIn](https://www.linkedin.com/in/ansu-john/)

---

## 🚀 Featured Projects

> Production-grade systems built to demonstrate senior Data Engineering capabilities across streaming, AI pipelines, observability, and data governance.

---

### 🛒 [Real-Time E-Commerce Data Pipeline](https://github.com/Ansu-John/realtime-ecommerse-data-pipeline)

An end-to-end **Modern Data Stack** pipeline delivering sub-minute latency from checkout event to BI dashboard.

- **Ingestion:** Python (Faker) on AWS EC2 → Aiven Apache Kafka (mTLS secured)
- **Processing:** PySpark Structured Streaming on Databricks → Delta Lake (Bronze)
- **Warehousing:** Python connector → Snowflake (Silver) with dbt transformations → Gold Marts
- **Design decisions:** Chose PySpark over SaaS ELT tools for true event-driven streaming with exactly-once semantics; implemented a Delta → Pandas → Snowflake REST pattern to work around Databricks Serverless DML restrictions

**Stack:** Python · Apache Kafka · PySpark · Databricks · Delta Lake · Snowflake · dbt · AWS EC2 · Aiven Cloud

---

### 🤖 [Unstructured Data Governance & RAG Pipeline](https://github.com/Ansu-John/Unstructured-data-governance-RAG)

An enterprise-grade **RAG pipeline and AI agent** for extracting complex financial and contractual data from unstructured PDFs, cataloging it in Snowflake, and serving intelligent answers via LangGraph.

- **Extraction:** PySpark + `pdfplumber` parses complex nested tables and checkboxes from PDFs stored in AWS S3
- **Cataloging:** Data loaded into Snowflake; embeddings generated via **Snowflake Cortex** (`e5-base-v2`) — data never leaves the secure database boundary
- **AI Agent:** LangGraph state machine routes queries to Cortex LLM (`llama3-70b`) for grounded, context-aware responses
- **Testing:** CI/CD-ready pytest suite with full mocking to validate pipeline logic without consuming database compute credits

**Stack:** Python · PySpark · AWS S3 · Snowflake · Snowflake Cortex · LangChain · LangGraph · Pytest

---

### 📄 [Intelligent Document Research Pipeline](https://github.com/Ansu-John/document-research-pipeline)

A **stateful, event-driven, observable AI workflow** that automates the full lifecycle of research document processing — from PDF upload to structured AI-generated synthesis.

- **API:** FastAPI returns `202 Accepted` instantly; heavy processing runs asynchronously via RabbitMQ
- **Worker:** FastStream consumer with exponential backoff, configurable retries, and a Dead Letter Queue (DLQ)
- **LangGraph pipeline:** Three nodes — Azure AI Document Intelligence (OCR + layout), OpenAI embeddings → Chroma/pgvector, GPT-4o synthesis with JSON-constrained outputs
- **Observability:** End-to-end Langfuse tracing on every LLM call, graph transition, and tool invocation
- **CI:** GitHub Actions — Ruff + Pyright + Pytest (80% coverage gate); all external services mocked

**Stack:** Python 3.12 · FastAPI · FastStream · RabbitMQ · LangGraph · Azure AI Document Intelligence · Azure Blob Storage · OpenAI · Chroma · pgvector · SQLAlchemy 2.0 · Langfuse

---

### 📊 [System Observer — Time-Series AI Observability Platform](https://github.com/Ansu-John/system-observer)

An intelligent observability platform that ingests system metrics into **TimescaleDB** and exposes an AI-powered diagnostic agent via FastAPI and the Model Context Protocol (MCP).

- **Ingestion:** Batch-ingest CPU, memory, disk, and network metrics into a TimescaleDB hypertable with automatic compression
- **Analytics:** Advanced SQL using `time_bucket`, `PERCENTILE_CONT`, `regr_slope`/`regr_r2` for windowed aggregations, outlier detection (Z-score), and trend analysis (linear regression)
- **AI Agent:** LangGraph supervisor with FastMCP tools classifies natural-language queries and returns structured diagnostic reports
- **Caching:** Redis 7 caches identical queries; duplicate requests are rate-limited (HTTP 429)
- **Production-ready:** Multi-stage Docker build, Kubernetes manifest (ArgoCD-ready), CI with Ruff + Pyright

**Stack:** Python 3.12 · FastAPI · TimescaleDB · SQLAlchemy 2.0 · LangGraph · FastMCP · Anthropic Claude · Redis · Docker · Kubernetes

---

## 🛠️ Core Skills

| Domain | Technologies |
|---|---|
| **Streaming & Pipelines** | Apache Kafka · PySpark Structured Streaming · Delta Lake · Databricks |
| **Data Warehousing** | Snowflake · Snowflake Cortex · dbt · TimescaleDB · PostgreSQL |
| **AI & LLM Pipelines** | LangGraph · LangChain · FastMCP · RAG · OpenAI · Anthropic Claude |
| **Cloud & Infrastructure** | AWS (S3, EC2) · Azure (Blob Storage, Document Intelligence) · Docker · Kubernetes |
| **APIs & Messaging** | FastAPI · RabbitMQ · FastStream · Redis |
| **Languages** | Python · Scala · SQL |
| **Quality & Observability** | Ruff · Pyright · Pytest · Langfuse · GitHub Actions |

---

## 📂 Other Projects

### ETL & Data Engineering
[ETL Verifier](https://github.com/Ansu-John/ETL-Verifier) — Post-load data validation after ETL using Scala.

[Big Data Analysis](https://github.com/Ansu-John/Big-Data-Analysis) — Spark RDD / DataFrame operations using PySpark 3.x.

### Machine Learning
[Feature Engineering with MLlib](https://github.com/Ansu-John/MLlib-Working-with-Features) · [Regression Models](https://github.com/Ansu-John/Regression-Models) · [Classification Models](https://github.com/Ansu-John/Classification-Models) · [Linear Regression with Spark](https://github.com/Ansu-John/Linear-Regression-with-Spark) · [Logistic Regression with Spark](https://github.com/Ansu-John/Logistic-Regression-with-Spark) · [Clustering](https://github.com/Ansu-John/ML-Clustering) · [Movie Recommender System](https://github.com/Ansu-John/Movie-Recommender-System)

### AI & Real-Life Projects
[Natural Language Processing](https://github.com/Ansu-John/Natural-Language-Processing) · [Credit Card Fraud Detection](https://github.com/Ansu-John/Credit-Card-Fraud-Detection) · [IBM HR Analytics — Employee Attrition](https://github.com/Ansu-John/IBM-HR-Analytics-Employee-Attrition) · [AB Testing](https://github.com/Ansu-John/AB-Testing) · [Customer Segmentation](https://github.com/Ansu-John/Customer-Segmentation) · [Retail Sales Forecasting](https://github.com/Ansu-John/Sales-Forecasting)

### Tutorials
[Study Notes](https://github.com/Ansu-John/Study-Materials) · [Introduction to Python](https://github.com/Ansu-John/Python)

---

💬 Feel free to message me on [LinkedIn](https://www.linkedin.com/in/ansu-john/) for any comments or collaboration opportunities.

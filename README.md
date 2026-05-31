<div align="center">

# Hey, I'm Muhammad Anas 👋

### Data Science Graduate · MLOps Engineer · Big Data Enthusiast

<p align="center">
  <a href="mailto:anashamid891@gmail.com"><img src="https://img.shields.io/badge/Gmail-D14836?style=for-the-badge&logo=gmail&logoColor=white"/></a>
  <a href="https://linkedin.com/in/anashamid12152004"><img src="https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white"/></a>
  <a href="https://github.com/ahcreative"><img src="https://img.shields.io/badge/GitHub-181717?style=for-the-badge&logo=github&logoColor=white"/></a>
  <img src="https://img.shields.io/badge/Location-Islamabad%2C%20Pakistan-green?style=for-the-badge&logo=googlemaps&logoColor=white"/>
</p>

<br/>

*Building scalable ML pipelines, real-time streaming systems, and production-grade MLOps infrastructure.*
*Currently pursuing BS Data Science at **FAST-NUCES, Islamabad**.*

<br/>

</div>

---

## 🧠 About Me

- 🎓 BS Data Science @ **FAST-NUCES Islamabad** (2022 – Present)
- 🔧 I build end-to-end ML systems — from raw data ingestion all the way to monitored, auto-retraining production deployments
- 🌊 Fascinated by real-time data streaming, drift detection, and making ML systems self-healing
- 📄 Published an **IEEE-style research paper** alongside my AutoDrift MLOps project
- 🤝 Open to collaborations on MLOps, data engineering, and applied ML projects

---

## 🛠️ Tech Stack

### Languages & ML Libraries
<p>
  <img src="https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white"/>
  <img src="https://img.shields.io/badge/C++-00599C?style=for-the-badge&logo=cplusplus&logoColor=white"/>
  <img src="https://img.shields.io/badge/SQL-4479A1?style=for-the-badge&logo=mysql&logoColor=white"/>
  <img src="https://img.shields.io/badge/Scikit--learn-F7931E?style=for-the-badge&logo=scikit-learn&logoColor=white"/>
  <img src="https://img.shields.io/badge/TensorFlow-FF6F00?style=for-the-badge&logo=tensorflow&logoColor=white"/>
  <img src="https://img.shields.io/badge/XGBoost-FF6600?style=for-the-badge&logoColor=white"/>
  <img src="https://img.shields.io/badge/Pandas-150458?style=for-the-badge&logo=pandas&logoColor=white"/>
  <img src="https://img.shields.io/badge/NumPy-013243?style=for-the-badge&logo=numpy&logoColor=white"/>
</p>

### MLOps & Infrastructure
<p>
  <img src="https://img.shields.io/badge/Docker-2496ED?style=for-the-badge&logo=docker&logoColor=white"/>
  <img src="https://img.shields.io/badge/FastAPI-009688?style=for-the-badge&logo=fastapi&logoColor=white"/>
  <img src="https://img.shields.io/badge/MLflow-0194E2?style=for-the-badge&logo=mlflow&logoColor=white"/>
  <img src="https://img.shields.io/badge/Apache_Airflow-017CEE?style=for-the-badge&logo=apacheairflow&logoColor=white"/>
  <img src="https://img.shields.io/badge/GitHub_Actions-2088FF?style=for-the-badge&logo=githubactions&logoColor=white"/>
  <img src="https://img.shields.io/badge/Prometheus-E6522C?style=for-the-badge&logo=prometheus&logoColor=white"/>
  <img src="https://img.shields.io/badge/Grafana-F46800?style=for-the-badge&logo=grafana&logoColor=white"/>
</p>

### Big Data & Streaming
<p>
  <img src="https://img.shields.io/badge/Apache_Kafka-231F20?style=for-the-badge&logo=apachekafka&logoColor=white"/>
  <img src="https://img.shields.io/badge/PySpark-E25A1C?style=for-the-badge&logo=apachespark&logoColor=white"/>
  <img src="https://img.shields.io/badge/Hadoop-66CCFF?style=for-the-badge&logo=apachehadoop&logoColor=black"/>
</p>

### Databases & Visualization
<p>
  <img src="https://img.shields.io/badge/PostgreSQL-4169E1?style=for-the-badge&logo=postgresql&logoColor=white"/>
  <img src="https://img.shields.io/badge/MongoDB-47A248?style=for-the-badge&logo=mongodb&logoColor=white"/>
  <img src="https://img.shields.io/badge/MySQL-4479A1?style=for-the-badge&logo=mysql&logoColor=white"/>
  <img src="https://img.shields.io/badge/Redis-DC382D?style=for-the-badge&logo=redis&logoColor=white"/>
  <img src="https://img.shields.io/badge/Power_BI-F2C811?style=for-the-badge&logo=powerbi&logoColor=black"/>
  <img src="https://img.shields.io/badge/Flask-000000?style=for-the-badge&logo=flask&logoColor=white"/>
</p>

---

## 🚀 Featured Projects

---

### 🔁 [AutoDrift — MLOps Pipeline with Automated Drift Detection](https://github.com/ahcreative/autodrift_mlops)
> `Python` `XGBoost` `FastAPI` `MLflow` `Docker` `Prometheus` `Grafana` `GitHub Actions`

A production-grade MLOps pipeline that detects data drift in real time and **triggers model retraining automatically** — zero human intervention required.

- Ran **3 drift detectors simultaneously** at the FastAPI inference layer:
  - 📊 **KS Test** — distribution comparison (most statistically grounded)
  - 📦 **PSI** — bucketed feature shift (detected drift earliest)
  - ⚡ **ADWIN** — adaptive change-point detection
  - Drift alert fires when **>30% of features** are flagged
- Evaluated across **5 progressively drifted batches** (UCI Credit Card, 30K records, 23 features) — all 3 detectors converged from batch 3 onward
- Retraining improved **F1: 0.5465 → 0.5513** · Drift check latency: **107ms avg (P95: 125ms)** · Inference: **1.8ms**
- 📄 Published a full **IEEE-style research paper** alongside the implementation

---

### ✈️ [End-to-End MLOps Pipeline — Titanic Survival Predictor](https://github.com/ahcreative)
> `Python` `Airflow` `MLflow` `Docker` `PostgreSQL` `Redis` `Scikit-learn`

Containerized ML pipeline with full orchestration, experiment tracking, and conditional model promotion.

- **7-service Docker Compose** stack: Airflow + MLflow + PostgreSQL + Redis (Celery broker)
- **10-task Airflow DAG** with parallel feature engineering (FamilySize, IsAlone, Title), XCom-based data passing, and auto-retry on validation failure
- `BranchPythonOperator` routes models to MLflow registry **only when evaluation thresholds are met**
- Resolved MLflow 3.x DNS rebinding security conflict in multi-container networks
- Designed race-condition-free parallel task architecture with automatic hyperparameter cycling
- Achieved **82%+ accuracy** on held-out test set

---

### 🏬 [Walmart Data Warehouse Prototype](https://github.com/ahcreative/Walmart-Data-Warehouse-Prototype)
> `Python` `SQL` `Power BI`

High-performance data warehouse with a custom ETL engine and executive BI dashboards.

- Built a custom **HYBRIDJOIN ETL pipeline** processing **550,000+ records** — cut runtime from hours to **under 10 minutes (>90% reduction)**
- Designed a complete **star schema** with 3 dimension tables and automated stored procedures enabling **20+ OLAP query paths**
- Connected **4 Power BI dashboards** with drill-downs, slicers, and executive KPIs — reduced complex report generation time by **~80%**

---

### 🎵 [Music Recommendation System](https://github.com/ahcreative/Music-recommendation-system)
> `Python` `Kafka` `MongoDB` `PySpark` `Flask`

Real-time recommendation engine backed by a live Kafka streaming pipeline.

- Extracted audio features (**MFCC, spectral centroid**) from thousands of MP3s using Librosa; applied PCA for storage optimization into MongoDB
- Trained **collaborative filtering (PySpark ALS)**, reading directly from MongoDB, evaluated via RMSE
- Wired **Apache Kafka** to stream real-time user activity from Flask frontend into the ML pipeline — live recommendation loop from interaction to prediction

---

### ⚡ [Energy Demand Forecasting](https://github.com/ahcreative/Energy-Demand-Forecasting)
> `Python` `ML` `LSTM` `PCA` `t-SNE`

Time-series forecasting with unsupervised clustering to improve accuracy on high-demand segments.

- Applied **PCA + t-SNE** to 10,000+ energy and weather records; evaluated K-Means, DBSCAN, Hierarchical clustering — identified **6 optimal clusters** via Silhouette Scores
- DBSCAN classified 94.85% of data as noise, revealing significant dataset sparsity
- Benchmarked **Linear Regression, Random Forest, XGBoost, and LSTM** using MAE, RMSE, MAPE
- Cluster-based training improved prediction accuracy on high-demand segments

---

### 📉 [Churn Prediction — Coursera Data Science Challenge](https://github.com/ahcreative/Coursera-Data-Science-Challenge-Churn-Prediction)
> `Python` `ML` `Feature Engineering`

- Engineered an **engagement ratio feature** that improved accuracy by ~15% over baseline
- Achieved **ROC-AUC 0.85+** on unseen test data

---

## 💼 Work Experience

**Data Scraping Intern** — *Evertise Digital, Islamabad* `Jan 2023 – Mar 2023`

- Built automated **Selenium bots** for end-to-end data collection
- Reduced manual acquisition time from hours to minutes — **~70% efficiency gain**

---

## 🎓 Education

**Bachelor of Science in Data Science** · FAST-NUCES, Islamabad `Aug 2022 – Present`

*Relevant Coursework:* Data Warehousing · MLOps · Data Visualization · Database Systems · Artificial Intelligence · Big Data Analytics · Probability & Advanced Statistics · Computer Networks · Parallel & Distributed Computing

---


<div align="center">

*"Building systems that learn, adapt, and heal themselves."*

⭐ If you find any of my projects useful, consider giving them a star!

</div>

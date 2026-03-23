<div align="center">

# 👋 Hello, I'm Yaniv

### Data Scientist & Analyst · Python · SQL · Spark · R · Tableau

*I believe every dataset has a story — my job is to find it.*

[![LinkedIn](https://img.shields.io/badge/LinkedIn-Connect-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white)](https://linkedin.com)

</div>

---

## 🧬 About Me

```python
yaniv = {
    "education"  : "B.Sc. Information Systems",
    "location"   : "Israel 🇮🇱",
    "focus"      : ["Data Science", "Big Data Engineering", "Analytics"],
    "languages"  : ["Python", "SQL", "R", "Scala (Spark)"],
    "tools"      : ["Pandas", "scikit-learn", "Spark", "Hadoop", "Tableau", "OpenCV"],
    "currently"  : "Building an automated end-to-end data analysis engine",
    "philosophy" : "Don't guess — measure. Don't describe — predict."
}
```

I work heavily with **Python and big data tools**, and love the ability to draw real, actionable conclusions from raw data. My projects span the full analytics lifecycle — from scraping the web and wrangling messy datasets, all the way to machine learning models, interactive dashboards, and distributed computing at scale with Spark & Hadoop.

---

## 🗂️ My Repositories — What Lives Here

| Repository | Description | Stack |
|---|---|---|
| 🔬 [**Data-Science**](https://github.com/yanivmm/Data-Science) | End-to-end DS projects: EDA, ML, NLP, feature engineering, automation | Python · Jupyter · scikit-learn |
| 🐍 [**python**](https://github.com/yanivmm/python) | Standalone Python scripts — utilities, automation, data pipelines | Python |
| 📊 [**R**](https://github.com/yanivmm/R) | Statistical analysis, decision tree optimization, modeling in R | R |
| 📈 [**tableau**](https://github.com/yanivmm/tableau) | Interactive business dashboards and visualization projects | Tableau |
| ⚡ [**spark**](https://github.com/yanivmm/spark) | Big data processing scripts using Apache Spark & Hadoop | PySpark · Hadoop · Jupyter |
| 🦠 [**Corona-scripts**](https://github.com/yanivmm/Corona-scripts) | COVID-19 data scraping, cleaning & time series analysis | Python · BeautifulSoup |

---

## ⚡ Tech Stack

<div align="center">

### 🐍 Python Ecosystem
![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)
![Pandas](https://img.shields.io/badge/Pandas-150458?style=for-the-badge&logo=pandas&logoColor=white)
![NumPy](https://img.shields.io/badge/NumPy-013243?style=for-the-badge&logo=numpy&logoColor=white)
![scikit-learn](https://img.shields.io/badge/scikit--learn-F7931E?style=for-the-badge&logo=scikit-learn&logoColor=white)
![OpenCV](https://img.shields.io/badge/OpenCV-5C3EE8?style=for-the-badge&logo=opencv&logoColor=white)
![Matplotlib](https://img.shields.io/badge/Matplotlib-11557c?style=for-the-badge)
![Seaborn](https://img.shields.io/badge/Seaborn-4c72b0?style=for-the-badge)
![BeautifulSoup](https://img.shields.io/badge/BeautifulSoup-59b347?style=for-the-badge)

### 🗄️ Data & Query
![SQL](https://img.shields.io/badge/SQL-Advanced-F29111?style=for-the-badge&logo=postgresql&logoColor=white)
![PostgreSQL](https://img.shields.io/badge/PostgreSQL-336791?style=for-the-badge&logo=postgresql&logoColor=white)

### ☁️ Big Data
![Apache Spark](https://img.shields.io/badge/Apache_Spark-E25A1C?style=for-the-badge&logo=apachespark&logoColor=white)
![Hadoop](https://img.shields.io/badge/Hadoop-66CCFF?style=for-the-badge&logo=apachehadoop&logoColor=black)

### 📊 BI & Visualization
![Tableau](https://img.shields.io/badge/Tableau-E97627?style=for-the-badge&logo=tableau&logoColor=white)
![Plotly](https://img.shields.io/badge/Plotly-3F4F75?style=for-the-badge&logo=plotly&logoColor=white)
![Jupyter](https://img.shields.io/badge/Jupyter-F37626?style=for-the-badge&logo=jupyter&logoColor=white)

### 📐 Statistics & Modeling
![R](https://img.shields.io/badge/R-276DC3?style=for-the-badge&logo=r&logoColor=white)
![NLTK](https://img.shields.io/badge/NLTK-4B8BBE?style=for-the-badge)
![TextBlob](https://img.shields.io/badge/TextBlob-6DB33F?style=for-the-badge)

</div>

---

## 🔬 Project Highlights

### 🤖 Data Science Automation Engine
> *[Data-Science repo](https://github.com/yanivmm/Data-Science) — flagship project*

Building a **dataset-agnostic EDA pipeline** that auto-detects column types, generates distribution plots, missing value reports, and correlation matrices — outputting a full analysis in one function call. The goal: one-click insights from any DataFrame.

```python
class AutoEDA:
    def __init__(self, df):
        self.num_cols  = df.select_dtypes(include='number').columns.tolist()
        self.cat_cols  = df.select_dtypes(include='object').columns.tolist()

    def run_full_report(self):
        self.missing_report()        # null heatmap
        self.plot_distributions()    # histograms per column
        self.correlation_heatmap()   # annotated corr matrix
        self.categorical_summary()   # top-N value counts
```

---

### ⚡ Apache Spark & Hadoop — Big Data Processing
> *[spark repo](https://github.com/yanivmm/spark)*

Processing datasets that don't fit in memory. Using **PySpark** for distributed transformations, aggregations, and ML pipelines — and **Hadoop HDFS** for distributed storage.

```python
from pyspark.sql import SparkSession
from pyspark.sql.functions import col, avg, window

spark = SparkSession.builder.appName("DataPipeline").getOrCreate()

# Distributed aggregation with window functions
df.groupBy(
    window(col("event_time"), "7 days"),
    col("category")
).agg(
    avg("value").alias("weekly_avg"),
    countDistinct("user_id").alias("unique_users")
).orderBy("window")
```

---

### 📊 Tableau Dashboards
> *[tableau repo](https://github.com/yanivmm/tableau)*

Interactive business dashboards translating complex datasets into clear visual narratives — KPI tracking, trend analysis, geographic heatmaps, and executive-level reporting.

---

### 📐 R — Statistical Modeling & Tree Optimization
> *[R repo](https://github.com/yanivmm/R)*

Decision tree construction and **pruning optimization** — finding the ideal tree complexity that minimizes cross-validation error without overfitting.

```r
library(rpart)
library(rpart.plot)

# Grow full tree, then prune to optimal CP
tree  <- rpart(target ~ ., data = train, method = "class", cp = 0)
opt   <- tree$cptable[which.min(tree$cptable[,"xerror"]), "CP"]
pruned_tree <- prune(tree, cp = opt)

rpart.plot(pruned_tree, type = 4, extra = 104)
```

---

### 🐍 Python Standalone Scripts
> *[python repo](https://github.com/yanivmm/python)*

Reusable utility scripts — file automation, data transformation pipelines, scheduled scrapers, and data ingestion tools designed for real-world use outside of notebooks.

---

## 🧩 Skills Radar

```
Python & Data Wrangling      ████████████████████  Expert
SQL & Query Optimization     ████████████████████  Expert
Feature Engineering          ███████████████████░  Advanced
Data Visualization           ███████████████████░  Advanced
Machine Learning             ████████████████░░░░  Advanced
Apache Spark / Big Data      ███████████████░░░░░  Advanced
Web Scraping & ETL           ████████████████████  Expert
R / Statistical Modeling     ████████████░░░░░░░░  Intermediate
NLP & Text Analysis          ████████████░░░░░░░░  Intermediate
Computer Vision (OpenCV)     ████████████░░░░░░░░  Intermediate
Tableau / BI Dashboards      ███████████████░░░░░  Advanced
```


---

## 🗺️ Domain Coverage

| Domain | Projects |
|---|---|
| 🏥 Public Safety & Policy | 911 Calls, Police Shootings, World Terrorism |
| 🦠 Epidemiology | COVID-19 Scraping & Analysis |
| 📸 Social Media Analytics | Instagram Scraper, YouTube Trending |
| 🎮 Business & Gaming | Video Game Sales, Sponsored Marketing |
| 🌍 Social Science | World Happiness Index, Global Indicators |
| 🍎 Health & Nutrition | Food & Vitamins Web Scraping |
| 👁️ Computer Vision | People Detection (OpenCV) |
| ⚡ Big Data Engineering | Spark & Hadoop distributed pipelines |
| 📊 Business Intelligence | Tableau Dashboards |

---

<div align="center">

*"Without data, you're just another person with an opinion."* — W. Edwards Deming

</div>

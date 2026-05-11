# Day-122-Pipeline-building

###  Overview

Day 122 focuses on **building a data pipeline** that automates the flow of data from source to destination.

A data pipeline helps in:

* Collecting data
* Transforming data
* Storing processed data
* Preparing data for analytics and machine learning

---

##  What is a Data Pipeline?

A data pipeline is a sequence of processes that moves and transforms data automatically.

---

##  Pipeline Workflow

```text id="pipe1"
Data Source → Ingestion → Transformation → Storage → Analytics/ML
```

---

##  Steps in Pipeline Building

### 1️ Data Ingestion

Collect data from:

* APIs
* CSV files
* Databases
* Streaming systems

---

### 2️ Data Transformation

Perform:

* Cleaning
* Filtering
* Aggregation
* Formatting

Example:

```python id="pipe2"
import pandas as pd

df = pd.read_csv("data.csv")

df.dropna(inplace=True)
```

---

### 3️ Data Storage

Store processed data in:

* SQL databases
* Cloud storage
* Data warehouses

---

### 4️ Automation

Schedule pipelines using:

* Apache Airflow
* Cron jobs
* Cloud schedulers

---

##  Simple ETL Example

```python id="pipe3"
import pandas as pd

# Extract
data = pd.read_csv("sales.csv")

# Transform
data["total"] = data["price"] * data["quantity"]

# Load
data.to_csv("processed_sales.csv", index=False)
```

---

##  Best Practices

- Build modular pipelines
- Add logging and monitoring
- Validate data quality
- Handle failures properly

---

##  Tools Commonly Used

* Python
* Apache Spark
* Airflow
* AWS / GCP

---

##  Key Takeaways

- Pipelines automate data workflows
- ETL is a core concept in Data Engineering
- Automation improves scalability and reliability

---


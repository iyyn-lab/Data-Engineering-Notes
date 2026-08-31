# Big Data Service Providers

## What is a Big Data Service Provider?

A Big Data service provider is a company that provides tools or platforms to help companies:

- Store huge amounts of data
- Process Big Data
- Run Hadoop and Spark
- Build data pipelines
- Manage Big Data infrastructure

Instead of building everything from scratch, companies can use these platforms.

---

# Major Big Data Service Providers

| Provider | Main Platform / Service | Simple Explanation |
|---|---|---|
| **Hortonworks** | HDP (Hortonworks Data Platform) | Hadoop-based platform |
| **Cloudera** | CDH / Cloudera Platform | Enterprise Hadoop and Big Data platform |
| **AWS** | EMR | Managed Hadoop and Spark service on AWS |
| **Microsoft Azure** | HDInsight / Azure Databricks | Managed Big Data and Spark services |
| **Google Cloud** | Dataproc | Managed Hadoop and Spark service on Google Cloud |
| **IBM** | BigInsights / Cloud Pak for Data | Enterprise Big Data and data platform |
| **Databricks** | Databricks Platform | Modern cloud platform built around Spark and Lakehouse |

---

# 1. Hortonworks

### HDP – Hortonworks Data Platform

Hortonworks provided a Hadoop-based platform.

It included technologies such as:

- Hadoop
- HDFS
- YARN
- Hive
- HBase
- Spark

### Important

Hortonworks later **merged with Cloudera in 2019**.

So Hortonworks is mainly important when learning the **history of Hadoop**.

```text
Hortonworks
     ↓
HDP
     ↓
Hadoop Ecosystem
```

---

# 2. Cloudera

Cloudera was one of the major Hadoop companies.

Its Hadoop distribution was commonly known as:

### CDH

Cloudera provided:

- Hadoop
- HDFS
- YARN
- Hive
- Impala
- HBase
- Spark

Cloudera and Hortonworks became one company after their merger in 2019.

Cloudera is still relevant, especially in large enterprise and hybrid/on-premise environments.

```text
Cloudera
    ↓
Hadoop + Big Data Platform
```

---

# 3. Amazon Web Services (AWS)

AWS provides managed Big Data services.

### Amazon EMR

**EMR = Elastic MapReduce**

EMR can run technologies such as:

- Hadoop
- Spark
- Hive
- HBase

Instead of building and maintaining a Hadoop cluster yourself, you can create a cluster using AWS.

Example:

```text
Data
 ↓
Amazon S3
 ↓
EMR / Spark
 ↓
Processed Data
```

---

# 4. Microsoft Azure

Microsoft Azure provides several services for Big Data.

### Azure HDInsight

HDInsight provides managed services for technologies such as:

- Hadoop
- Spark
- Hive
- Kafka

Azure also provides:

### Azure Databricks

This is a managed Databricks platform integrated with Azure.

Modern Azure data engineering commonly uses:

```text
Azure Data Lake Storage
        ↓
Azure Databricks
        ↓
Spark
```

---

# 5. Google Cloud

Google Cloud provides:

### Dataproc

Dataproc is a managed service for running:

- Hadoop
- Spark
- Hive

You don't have to manually build the entire cluster.

Example:

```text
Google Cloud Storage
        ↓
Dataproc / Spark
        ↓
BigQuery
```

---

# 6. IBM

IBM has provided enterprise Big Data platforms.

### IBM BigInsights

BigInsights was an IBM Hadoop-based platform.

IBM's modern data platform offerings include:

### Cloud Pak for Data

It provides capabilities for:

- Data management
- Data integration
- Analytics
- AI
- Data governance

IBM is mainly seen in large enterprise environments.

---

# 7. Databricks

Databricks is one of the most important modern data platforms.

It was founded by the creators of **Apache Spark**.

Databricks provides:

- Apache Spark
- Lakehouse architecture
- Data engineering
- SQL analytics
- Machine Learning
- AI capabilities

Simple idea:

```text
Data
 ↓
Cloud Storage
 ↓
Databricks / Spark
 ↓
Analytics / AI
```

Databricks is very important for modern Data Engineering.

---

# Old vs Modern Big Data Platforms

## Earlier Hadoop Era

The major names were:

```text
Hortonworks
Cloudera
MapR
IBM BigInsights
```

The main focus was:

```text
Hadoop
HDFS
YARN
MapReduce
Hive
```

---

## Modern Cloud Era

Today, Big Data workloads are increasingly built using:

```text
AWS EMR
Google Dataproc
Azure Databricks
Databricks
Cloud Storage
Apache Spark
```

The focus has moved toward:

```text
Cloud
 +
Spark
 +
Data Lakes
 +
Lakehouse
 +
Analytics
 +
AI
```

---

# Easy Way to Remember

```text
Hadoop Era
│
├── Hortonworks → HDP
├── Cloudera    → CDH
└── IBM         → BigInsights
        ↓
    Hadoop Ecosystem
        ↓
Cloud Era
│
├── AWS         → EMR
├── Google      → Dataproc
├── Azure       → HDInsight / Databricks
└── Databricks  → Spark + Lakehouse
```

---

# Important Names to Remember

For your Data Engineering studies, remember these first:

### Hadoop / Historical

```text
Hortonworks → HDP
Cloudera    → CDH
IBM         → BigInsights
```

### Cloud

```text
AWS         → EMR
Google      → Dataproc
Azure       → HDInsight
```

### Modern Data Engineering

```text
Databricks → Spark + Lakehouse
```

> **Simple conclusion:** Hadoop was heavily associated with on-premise Big Data platforms such as Hortonworks and Cloudera. Today, Big Data workloads have increasingly moved to cloud platforms and Spark-based systems such as Databricks, AWS EMR, Google Dataproc, and Azure Databricks.
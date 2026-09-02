# Hadoop Ecosystem - Simple Notes

## History of Hadoop

### 2002 - Google File System (GFS)

Google created **Google File System (GFS)** to store huge amounts of data across multiple machines.

### 2003 - Google MapReduce (GMR)

Google created **MapReduce** to process large amounts of data in parallel across multiple machines.

### Basic Idea

```text
GFS       -> Store Data
MapReduce -> Process Data
```

Google's idea was:

1. Store data in a distributed way using GFS.
2. Process data in a distributed way using MapReduce.

---

## Birth of Hadoop

Around **2005-2006**, the Hadoop project was created based on Google's GFS and MapReduce concepts.

### Creator of Hadoop

**Doug Cutting** invented Hadoop.

He is known as the **Father of Hadoop**.

Later, Hadoop was released as an open-source project through the **Apache Software Foundation (ASF)**.

---



# Hadoop Framework

A **Framework** is a collection of multiple components working together.

Initially Hadoop contained only two major components:

## 1. HDFS

**Hadoop Distributed File System**

Purpose:

- Stores data across multiple machines.
- Provides distributed storage.



## 2. MapReduce

Purpose:

- Processes data in parallel.
- Allows distributed computation.

```text
Hadoop
│
├── HDFS
│   └── Storage
│
└── MapReduce
    └── Processing
```

These were the first two Hadoop components.

---



# Why Hive Was Created

Facebook started using Hadoop.

They liked Hadoop, but there was a problem.

MapReduce jobs were mostly written in Java.

Many Facebook developers were comfortable with SQL but not Java.

Example:

```text
SQL -> 1 line query

Java -> 4-5 lines of code
```

Facebook wanted a simpler way to work with Hadoop.

---



# Hive

Facebook created **Hive**.

Hive is called a **Query Engine**.

Instead of writing Java code, users can write SQL queries.

```text
SQL Query
     ↓
Hive
     ↓
Converts internally java to MapReduce
     ↓
Execution
```

Benefits:

- Developers can use SQL.
- No need to write MapReduce code manually.
- Easier to learn and use.

This is one reason why people say:

> For Hadoop, SQL knowledge is very important.

---



# Pig

Pig was created by **Yahoo**.

Yahoo developers wanted something easier than Java and SQL.

They created a scripting language called:

**Pig Latin**

Example Flow:

```text
Pig Latin Script
        ↓
Pig
        ↓
Converts to Java to MapReduce
        ↓
Execution
```

Benefits:

- Easier than Java.
- Good for data processing scripts.

---



# Sqoop

Sqoop was developed by contributors from different organizations.

Purpose:

Move data between:

```text
RDBMS ↔ Hadoop
```

Examples of RDBMS:

- MySQL
- Oracle
- SQL Server
- PostgreSQL

---



## Why Sqoop?

Without Sqoop, developers would need to write MapReduce code to connect databases.

Sqoop automates this process.

---



## Sqoop Import

Move data from:

```text
RDBMS
   ↓
Hadoop
```

---



## Sqoop Export

Move data from:

```text
Hadoop
   ↓
RDBMS
```

---



## Sqoop Commands

Sqoop is not a programming language.

It uses commands similar to Linux commands.

Example:

```bash
sqoop import
sqoop export
```

Internally, Sqoop uses MapReduce.

---



## Where Can Sqoop Store Imported Data?

Data imported from RDBMS can be stored in:

1. HDFS
2. Hive
3. HBase

```text
       RDBMS
        ↓
 ┌───────┬───────┬
 ↓       ↓       ↓
HDFS    Hive    HBase
```

---



## Where Can Sqoop Read From?

Sqoop can export data from:

1. HDFS
2. Hive

Back into an RDBMS.

HBase support is limited because HBase is a NoSQL database and its structure is different from relational databases.

---



# Oozie

Oozie was created by Yahoo.

Purpose:

**Job Scheduling and Automation**

Example:

You have a Hive query.

You want it to run:

- Every day at 2 AM
- Every week
- Every month

Oozie can schedule it automatically.

```text
Hive Query
      ↓
Oozie Scheduler
      ↓
Runs Automatically
```

Oozie internally uses Java.

---



# Components Dependent on MapReduce

The following Hadoop ecosystem components depend on MapReduce:

```text
Hive
Pig
Sqoop
Oozie
```

These are often called:

> Abstractions of MapReducer

Without MapReduce, these components cannot perform their core processing.

---



# HBase

HBase is a **NoSQL Database**.

It is often called:

> Hadoop Database

Characteristics:

- Designed for Hadoop.
- Hadoop is required.
- MapReduce is optional.

```text
Hadoop
   ↓
 HBase
```

Purpose:

Store huge volumes of data with fast access.

---



# Mahout

Mahout is used for:

- Machine Learning
- Artificial Intelligence
- Data Science

Examples:

- Recommendation systems
- Clustering
- Classification

---



# Flume

Flume is a data ingestion tool.

Purpose:

Collect and move data into Hadoop.

---



## What Can Flume Read?

Flume can collect data from:

- Log files
- Folders
- Web servers
- Application servers
- Social media events
- Streaming event sources

Example:

```text
Web Server
     ↓
   Flume
     ↓
  Hadoop
```

---



## Flume vs Sqoop



### Sqoop

```text
RDBMS ↔ Hadoop
```

Supports both import and export.

### Flume

```text
Source → Hadoop
```

Only imports data into Hadoop.

No export capability.

---



# Important Concept: Streaming vs Stream Processing

Many people misunderstand Flume.

They think Hadoop supports real-time stream processing because Flume handles streams.

This is incorrect.

---



## Real-Time Streaming Retrieval

Example:

```text
ATM Transaction
      ↓
Flume Captures Event
```

Flume only collects the event.

---



## Real-Time Stream Processing

Example:

```text
ATM Transaction
      ↓
Immediately Processed
      ↓
Response Generated
```

This is true stream processing.

---



## Hadoop's Limitation

Flume can collect real-time data.

However:

```text
Processing
     ↓
MapReduce / Hive
```

MapReduce is batch-oriented.

So Hadoop supports:

- Real-time data collection

But not:

- Real-time stream processing

---



# Major Hadoop Ecosystem Components

```text
Hadoop Core
│
├── HDFS
├── MapReduce
│
├── Hive
├── Pig
├── Sqoop
├── Oozie
├── HBase
├── Mahout
└── Flume
```

These are some of the most commonly used Hadoop ecosystem components.

---



# Hadoop Framework vs Hadoop Ecosystem



### Hadoop Framework

Core Hadoop components:

```text
HDFS
MapReduce
```



### Hadoop Ecosystem

Includes:

```text
Hive
Pig
Sqoop
Oozie
HBase
Mahout
Flume
HDFS
MapReduce
```

---



# Two Very Important Characteristics

These concepts apply not only to Hadoop but to most Big Data frameworks.

---



## 1. Loosely Coupled Architecture

Components are independent.

Example:

If a project does not need Hive:

```text
Remove Hive
     ↓
Hadoop Still Works
```

Similarly:

- Pig can be removed.
- Oozie can be removed.
- Flume can be removed.

The core components are:

```text
HDFS
MapReduce
```

Most projects do not use every Hadoop component.

Different projects use different combinations.

---



## 2. Easy Integration with Other Technologies

Big Data frameworks can integrate with other frameworks.

Example:

```text
Hadoop ↔ Spark
```

Hadoop can also integrate with:

- RDBMS
- ETL Tools
- Mainframe Systems
- Data Science Tools
- Testing Frameworks
- Existing Enterprise Applications

This makes migration easier.

Organizations can continue using existing systems while gradually adopting Big Data technologies.

---



# Summary

```text
Google GFS        → Inspired HDFS
Google MapReduce  → Inspired Hadoop MapReduce

Doug Cutting      → Created Hadoop

HDFS              → Storage
MapReduce         → Processing

Hive              → SQL on Hadoop
Pig               → Pig Latin Scripts
Sqoop             → RDBMS ↔ Hadoop
Oozie             → Scheduling
HBase             → NoSQL Database
Mahout            → Machine Learning
Flume             → Data Ingestion

Key Features:
✓ Distributed Storage
✓ Distributed Processing
✓ Loosely Coupled Architecture
✓ Easy Integration with Other Technologies
```


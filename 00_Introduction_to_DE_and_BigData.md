# What is Data Engineering? What is Big Data?

## Understanding Data

Data is simply a collection of information.

Examples:

- Customer names
- Orders
- Bank transactions
- Website clicks
- Images
- Videos
- Sensor readings

As humans:

```text
Information → Brain → Processing → Result
```

Our brain:

1. Stores information
2. Processes information
3. Produces results

Computers do something similar:

```text
Data → Storage → Processing → Output
```

- Storage = Keeping data safely
- Processing = Working on data to produce useful results

---

# What is Data Engineering?

Data Engineering is the field that focuses on:

- Collecting data
- Storing data
- Moving data
- Cleaning data
- Processing data
- Transforming data
- Delivering data to users and applications

In simple words:

> Data Engineering is the practice of solving data-related problems using technology.

A Data Engineer's job is to ensure that data is available, reliable, and usable for businesses.

---

# Simple Example

Imagine an e-commerce company.

Customers:

- Place orders
- Make payments
- Track deliveries

All these activities generate data.

A Data Engineer builds systems that:

```text
Collect Data
      ↓
Store Data
      ↓
Process Data
      ↓
Generate Useful Information
```

---

# What Problems Can Data Have?

Not all data is easy to work with.

Sometimes data creates problems during:

- Storage
- Processing
- Movement
- Quality checking
- Analysis

Let's see some examples.

---

# Scenario 1: Storage and Processing Problems

Suppose we receive extremely large amounts of data.

```text
Huge Data
   ↓
Hard to Store
   ↓
Hard to Process
```

Problems:

- Storage becomes expensive
- Processing becomes slow
- Systems may crash

In this case:

```text
Storage Problem + Processing Problem
```

---

# Scenario 2: Processing Problem Only

Suppose storage is not an issue.

We can store the data.

However:

```text
Data is Stored
      ↓
Processing Takes Too Long
```

Problems:

- Reports take hours
- Queries become slow
- Analytics become difficult

In this case:

```text
Processing Problem
```

---

# Scenario 3: Storage Problem Only

Suppose data can be processed easily.

But storing it becomes difficult.

Problems:

- Storage cost increases
- Storage systems become overloaded

In this case:

```text
Storage Problem
```

---

# What is Big Data?

Many people think:

> Big Data means very large data.

That is only partially correct.

A better definition is:

> Big Data refers to data that creates challenges for traditional systems.

The challenge may be:

- Size
- Speed
- Complexity
- Quality
- Processing
- Storage
- Analysis

In simple words:

> If normal systems struggle to handle the data, it becomes a Big Data problem.

---

# Big Data is a Problem Statement

Big Data is not a single technology.

Big Data is a collection of data challenges.

Example:

```text
Data Problem
      ↓
Need Better Solution
      ↓
Use Big Data Technologies
```

---

# The Famous 3 V's of Big Data

The market often explains Big Data using the "3 V's".

---

## 1. Volume

Volume means the amount of data.

Example:

```text
1 GB
100 GB
10 TB
100 TB
```

The larger the data, the harder it becomes to store and process.

---

## 2. Velocity

Velocity means the speed at which data arrives.

Examples:

- Stock market data
- Payment transactions
- Website clicks
- IoT sensor data

Data may arrive every second or even every millisecond.

---

## 3. Variety

Variety means different types of data.

### Structured Data

Organized data.

Example:

```text
CSV Files
Database Tables
Excel Sheets
```

---

### Semi-Structured Data

Partially organized.

Example:

```text
JSON
XML
Application Logs
```

---

### Unstructured Data

No fixed format.

Example:

```text
Audio Files
Video Files
Images
Documents
```

Handling all these different formats creates challenges.

---

# Are There Only 3 V's?

No.

The market commonly teaches:

```text
Volume
Velocity
Variety
```

But over time more V's were added.

Examples:

- Veracity
- Value
- Variability
- Visualization

Today there are many V's discussed in the industry.

---

# Does Big Data Have a Fixed Size?

No.

There is no official rule such as:

```text
100 GB = Big Data
```

or

```text
1 TB = Big Data
```

A dataset may be considered Big Data if existing systems cannot handle it efficiently.

Big Data depends on the problem, not a fixed size.

---

# What Problems Can Big Data Solve?

Many people think Big Data is only for storage problems.

That is incorrect.

Big Data solutions can help solve:

- Storage problems
- Processing problems
- Performance problems
- Data movement problems
- Scalability problems
- Analytics problems

Volume is only one type of problem.

---

# Popular Big Data Technologies

There are many Big Data technologies available.

The two most popular and influential technologies are:

## Hadoop

Provides:

- Distributed Storage
- Distributed Processing
- Cluster Management

---

## Spark

Provides:

- Fast Distributed Processing
- In-Memory Computing
- SQL Processing
- Machine Learning Support
- Streaming Support

Today Spark is one of the most widely used Big Data processing engines.

---

# Hadoop and Spark are Not the Entire Big Data World

Many people think:

```text
Big Data = Hadoop + Spark
```

This is not completely true.

Big Data contains many tools and technologies.

Examples:

- Hadoop
- Spark
- Kafka
- Flink
- Hive
- Airflow
- Databricks
- Snowflake

Hadoop and Spark are simply two of the most popular solutions.

---

# What is Data Engineering Then?

Data Engineering is a broader domain.

Inside Data Engineering we have many technologies:

- Oracle
- MySQL
- PostgreSQL
- Informatica
- Hadoop
- Spark
- Kafka
- Airflow
- Databricks

All of these are Data Engineering technologies.

---

# Is Data Engineering Only Big Data?

No.

A Data Engineer does not necessarily need to work only on Big Data.

Examples:

A Data Engineer may work with:

- Oracle
- MySQL
- SQL Server
- Informatica
- ETL Tools
- Cloud Platforms
- Hadoop
- Spark

All of these are Data Engineering work.

---

# Why Do People Associate Data Engineering with Big Data?

Because Big Data technologies are currently among the most popular technologies in the market.

Therefore many people automatically assume:

```text
Data Engineer = Hadoop + Spark
```

But Data Engineering is much larger than Big Data.

---

# What Does a Data Engineer Actually Do?

A Data Engineer solves data problems using technology.

Typical responsibilities:

### SQL

- Writing queries
- Data analysis
- Data transformation

### Programming

- Python
- Java
- Scala

### Linux

- Shell commands
- Automation
- Server management

### Data Pipelines

- Moving data
- Scheduling jobs
- Monitoring workflows

### Big Data

- Hadoop
- Spark
- Kafka

---

# Is SQL Alone Enough?

No.

SQL is very important.

However Data Engineering is not only SQL.

A Data Engineer usually needs:

```text
SQL
+
Programming
+
Linux
+
Data Technologies
```

In many projects:

- SQL is heavily used
- Coding is also required
- Automation is important

A strong Data Engineer understands both SQL and programming.

---

# Final Definition

## Data Engineering

> Data Engineering is the discipline of collecting, storing, moving, processing, transforming, and delivering data by using various technologies to solve business and technical data problems.

## Big Data

> Big Data refers to data-related challenges that traditional systems struggle to handle efficiently. These challenges may involve volume, velocity, variety, processing, storage, scalability, or other data-related problems.

---

# Relationship Between Data Engineering and Big Data

```text
Data Engineering
│
├── SQL Databases
├── Oracle
├── MySQL
├── Informatica
├── ETL Tools
├── Cloud Platforms
├── Big Data
│     ├── Hadoop
│     ├── Spark
│     ├── Kafka
│     └── Flink
│
└── Analytics Systems
```

Big Data is a part of Data Engineering.

Data Engineering is the broader domain.

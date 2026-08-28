# Data Engineering & Big Data - Introduction

## 1. What is Data?
- Data is simply a collection of information.
- **Analogy:** As humans, we store data in our brains. We process the data in our brain to produce an outcome or a decision.
- In the computer world, we do the same thing: 
  1. Store data (Storage).
  2. Process data (Processing/Computing).
  3. Generate a result (Output).

---

## 2. What is "Big Data"?
When we have a problem with data (either storing it or processing it), it is called **Big Data**. 

**Important Concept:** Big Data is **not** just a specific size (like "1 Terabyte"). It is a **Problem Statement**. 

### The 3 Main Scenarios (The "Problems")
1. **Scenario 1:** The data is too large. We cannot store it, and we cannot process it. (Problem in both Storage and Processing).
2. **Scenario 2:** We can store the data (with difficulty), but processing it takes too much time. (Problem in Processing).
3. **Scenario 3:** Storing the data is a huge problem, but processing is easy. (Problem in Storage).

**Conclusion:** Whenever you face a problem in handling data (whether it's storing or processing), that is called **Big Data**.

---

## 3. The "V's" of Big Data
To categorize these problems, the industry labeled them using "V's". 

### The Original 3 V's:
- **Volume:** The problem of **Storage**. (Data is too big to fit in normal storage).
- **Velocity:** The problem of **Speed**. (Data is coming too fast, or takes too long to process).
- **Variety:** The problem of **Different Structures**.
  - **Structured Data:** Excel files, CSV files (Rows and Columns).
  - **Semi-Structured Data:** Log files, JSON, XML (Has some structure, but not fixed tables).
  - **Unstructured Data:** Audio, Video, Images (No fixed structure).

### The Additional 2 V's (Modern Big Data):
- **Veracity:** The problem of **Trust/Accuracy**. (Is the data clean or messy?).
- **Value:** The problem of **Business Worth**. (How do we turn this huge data into money or useful insights?).

---

## 4. How do we solve Big Data problems?
- There are 50+ tools and domains to solve Big Data problems.
- **Top Leading Solutions:** 
  1. **Hadoop** (Legacy batch processing).
  2. **Spark** (Modern, fast, distributed processing).
- Both Hadoop and Spark have their own internal components.

**Note:** Big Data tools do **not** just solve the "Volume" problem. They also solve Velocity (Streaming), Variety (handling images/JSON), and Value (Analytics).

---

## 5. What is Data Engineering?
- **Definition:** Data Engineering is a **Domain** (a career field) that solves any problem related to data using technology.
- **Scope:** A Data Engineer does not only work on Big Data. They work with *all* data technologies.
  - Example tools inside Data Engineering: Oracle, MySQL, Informatica, Hadoop, Spark, Snowflake, etc.
- **Market Reality:** The industry often assumes a Data Engineer knows Big Data (like Spark), because it is the top technology. 
- **The Job:** A Data Engineer solves problems related to data (ingestion, cleaning, transformation, storage) using Python, SQL, and various data tools.

---

## 6. The Daily Work of a Data Engineer
- A Data Engineer writes **code** (Python).
- A Data Engineer uses **Linux commands** (to manage servers and files).
- A Data Engineer writes **SQL** queries extensively.
- **The 50/50 Rule:** 
  - ~50% of your work is writing SQL queries.
  - ~50% of your work is writing code (Python/Spark) and configuring pipelines.

**Goal:** A Data Engineer's job is to find *any* solution for *any* data problem. 

**Final Thought:** Data Engineering is an **Evergreen field** because data will always exist, and someone will always need to manage it.
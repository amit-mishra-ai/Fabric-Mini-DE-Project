# 📊 Microsoft Fabric Mini Project – End-to-End Data Pipeline (GitHub → Lakehouse → Power BI)

## 🚀 Project Overview
This mini project demonstrates an end-to-end data engineering workflow built using **Microsoft Fabric**. The goal was to fetch data directly from a GitHub repository, load it into a Lakehouse architecture, transform it for analytics, and finally create a Power BI report for insights.

The project follows a **Bronze → Silver architecture**, uses pipeline automation, and applies data cleaning and transformation techniques to prepare a semantic model for reporting.

This project helped me gain hands-on experience with real-world data engineering concepts such as data ingestion, pipeline orchestration, transformation, and reporting.

---

## 🎯 Objectives
- Fetch data from GitHub using Microsoft Fabric pipelines
- Store raw data in the Bronze Lakehouse
- Clean and transform data into the Silver layer
- Build a semantic model for reporting
- Create a Power BI report for visualization
- Automate file ingestion using Lookup and ForEach activities

---

## 🏗️ Architecture Overview
The project follows a layered Lakehouse architecture:

**GitHub (Source) → Fabric Pipeline → Bronze Lakehouse → Data Cleaning → Silver Tables → Semantic Model → Power BI Report**

---

## ⚙️ Pipeline Workflow

### 1️⃣ Data Ingestion from GitHub
- Used a **Lookup activity** to read a JSON file containing file details from GitHub.
- If the lookup was successful, a **ForEach loop** was triggered.
- Inside the ForEach loop:
  - A **Copy Data activity** was executed
  - Each file was copied individually from GitHub to the Bronze Lakehouse

### 2️⃣ Bronze Layer (Raw Data)
- Stored raw, unprocessed data
- Maintained original structure for traceability

### 3️⃣ Silver Layer (Cleaned Data)
- Cleaned and transformed the data
- Removed inconsistencies and null values
- Structured the dataset for analytics

### 4️⃣ Semantic Model
- Built a semantic model to enable reporting
- Defined relationships and measures for analysis

### 5️⃣ Power BI Reporting
- Created a simple Power BI report
- Visualized key insights from the cleaned dataset

---

## 🛠️ Tools & Technologies Used
- **Microsoft Fabric**
- Fabric Pipelines
- Lakehouse Architecture
- GitHub (Data Source)
- Power BI
- JSON Configuration
- Data Transformation Techniques


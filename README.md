# 💊 Digital Prescription Record Analysis – P1

![Python](https://img.shields.io/badge/Python-3.x-blue)
![MySQL](https://img.shields.io/badge/MySQL-Database-orange)
![ETL](https://img.shields.io/badge/ETL-Pipeline-green)
![Healthcare](https://img.shields.io/badge/Domain-Healthcare-red)

---

## 📌 Project Overview

Digital Prescription Record Analysis is a Healthcare Informatics project designed to digitize, clean, validate, store, and analyze medical prescription records.

The system implements an automated ETL pipeline using Python and stores structured, validated data in MySQL for analytical querying and visualization.

---

## 🎯 Objectives

- Reduce prescription errors through strict validation
- Digitize prescription record management
- Ensure secure and structured data storage
- Enable analytical insights for healthcare monitoring
- Improve overall data quality using business rules

---

## 🏗️ System Architecture

```
Raw CSV Files
        ↓
Python ETL (Pandas)
   • Deduplication
   • Null Handling
   • Business Rule Validation
        ↓
MySQL Database
   • Clean Tables
   • Constraints Applied
        ↓
SQL Analytics
        ↓
Matplotlib / Seaborn Dashboards
```

---

## 🛠️ Tech Stack

| Technology | Usage |
|------------|--------|
| Python | ETL Processing |
| Pandas | Data Cleaning & Transformation |
| MySQL | Relational Data Storage |
| SQL | Analytical Queries |
| Matplotlib | Data Visualization |
| Seaborn | Advanced Visualization |

---

## 📂 Project Structure

```
Digital-Prescription-P1/
│
├── data/
│   ├── doctors_1000.csv
│   ├── patients_1000.csv
│   ├── medicines_1000.csv
│   └── prescriptions_1000.csv
│
├── etl_pipeline.py
├── analytics_queries.sql
├── dashboards.py
├── requirements.txt
└── README.md
```

---

## ⚙️ Business Rules Implemented

- Age must be between 0–100
- Duplicate prescriptions are invalid
- Prescriptions without valid patient/doctor are rejected
- Missing dosage/frequency → "Not Provided"
- Unknown gender → "U"

---

## 🔄 ETL Pipeline Details

### 1️⃣ Extract
- Load raw CSV datasets using Pandas

### 2️⃣ Transform
- Remove duplicate records
- Handle missing values
- Apply business rules
- Validate foreign key relationships
- Standardize formats

### 3️⃣ Load
- Insert cleaned data into MySQL
- Apply primary key and foreign key constraints
- Enforce NOT NULL conditions

---

## 📊 Analytics & Insights

- Most frequently prescribed medicines
- Doctor-wise prescription volume comparison
- Gender-wise prescription distribution
- Age group vs number of prescriptions
- Detection of unusually high-prescribing doctors (IQR method)
- Daily prescription trends
- Data quality comparison (Before vs After Cleaning)

---

## 🚀 Installation & Setup

### 1️⃣ Clone Repository

```bash
git clone https://github.com/your-username/Digital-Prescription-P1.git
cd Digital-Prescription-P1
```

### 2️⃣ Install Dependencies

```bash
pip install -r requirements.txt
```

### 3️⃣ Configure Database

- Create MySQL database
- Update database credentials inside `etl_pipeline.py`

### 4️⃣ Run ETL Pipeline

```bash
python etl_pipeline.py
```

### 5️⃣ Run Dashboards

```bash
python dashboards.py
```

---

## 🧪 Data Quality Validation

- Missing value comparison (Before vs After)
- Outlier detection using IQR
- Referential integrity validation
- Constraint enforcement at database level

---

## 🔐 Data Integrity Measures

- Primary Key Constraints
- Foreign Key Constraints
- NOT NULL Enforcement
- Business Rule Validation
- Duplicate Removal

---

## 📈 Sample Output

- Clean MySQL tables
- Terminal-based analytical summaries
- Graphical dashboards using Matplotlib

---

## 📚 Learning Outcomes

- Real-world ETL pipeline implementation
- Data cleaning and validation techniques
- Relational database design
- SQL-based analytics
- Data visualization in Python
- Healthcare data quality management

---

## 👨‍💻 Author

Mahender Reddy  
Data Engineering Project  
Healthcare Informatics  

---

## 📄 License

This project is developed for academic and learning purposes.

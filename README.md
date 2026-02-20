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
Matplotlib 
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

---

## 📂 Project Structure

```
Digital-Prescription-P1/
│
│── doctors_1000.csv
│── patients_1000.csv
│── medicines_1000.csv
│── prescriptions_1000.csv
├── Digital Prescription Record Analysis-P1.py
├── Digital Prescription Record Analysis DDL.txt
├── Digital Prescription Record Analysis.docx
├── Digital Prescrption Problem statement_with_Business Rules _Business Insights.txt
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

## 📈 Sample Outputs
<img width="554" height="516" alt="download" src="https://github.com/user-attachments/assets/b897e035-7261-420c-9bb0-a9b04c9fbada" />
<img width="554" height="505" alt="download" src="https://github.com/user-attachments/assets/49f773e7-70e8-4ab6-8e0a-dbd1c3ef2519" />

<img width="389" height="409" alt="download" src="https://github.com/user-attachments/assets/e2a95375-164a-4fc9-9ef4-6ef318cc80c6" />
<img width="989" height="490" alt="download" src="https://github.com/user-attachments/assets/2aafa606-7584-45de-9060-6f0a42e62282" />
<img width="580" height="433" alt="download" src="https://github.com/user-attachments/assets/ad1b1c89-3ea3-4cbe-b9cc-ba221c8a27fd" />
<img width="571" height="453" alt="download" src="https://github.com/user-attachments/assets/e0427d87-5892-49b4-9611-cdc1df148a75" />
<img width="989" height="490" alt="download" src="https://github.com/user-attachments/assets/6a0e6644-ab32-4b20-bf47-a13afdf6ee83" />
<img width="690" height="390" alt="download" src="https://github.com/user-attachments/assets/09860d84-c7bb-4f65-a131-cf007d4ee9c5" />

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
Data Engineering Project (Python+SQL) 
Healthcare Informatics  

---

## 📄 License

This project is developed for academic and learning purposes.

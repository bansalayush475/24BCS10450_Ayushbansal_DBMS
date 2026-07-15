# 🏥 Experiment 1: Hospital Management System

![SQL](https://img.shields.io/badge/Language-SQL-blue)
![Database](https://img.shields.io/badge/Database-RDBMS-green)
![Status](https://img.shields.io/badge/Experiment-Completed-success)

## 📌 Overview

This experiment demonstrates how to populate a **Hospital Management System** database using SQL `INSERT` statements and retrieve records using `SELECT` queries.

The experiment covers:

- Inserting data into multiple related tables
- Maintaining relationships using Primary & Foreign Keys
- Retrieving the first record from selected tables
- Understanding basic SQL DML operations

---

# 📂 Database Tables

The database consists of the following six tables:

| Table Name | Description |
|------------|-------------|
| Doctors | Stores doctor information |
| Patients | Stores patient details |
| Appointments | Stores appointment schedules |
| Treatments | Stores treatment information |
| MedicalRecords | Stores patient medical records |
| Billing | Stores billing information |

---

# 📊 Database Schema

```
Doctors
│
├── DoctorID (PK)
├── Name
├── Specialization
├── ContactNumber
└── Email

Patients
│
├── PatientID (PK)
├── Name
├── DOB
├── Gender
├── ContactNumber
└── Address

Appointments
│
├── AppointmentID (PK)
├── PatientID (FK)
├── DoctorID (FK)
├── AppointmentDate
└── Status

Treatments
│
├── TreatmentID (PK)
├── PatientID (FK)
├── DoctorID (FK)
├── Diagnosis
├── TreatmentDescription
└── TreatmentDate

MedicalRecords
│
├── RecordID (PK)
├── PatientID (FK)
├── TreatmentID (FK)
├── Notes
└── RecordDate

Billing
│
├── BillID (PK)
├── PatientID (FK)
├── TreatmentID (FK)
├── Amount
├── BillDate
└── Status
```

---

# 🎯 Objectives

- Populate database tables using SQL.
- Learn how to insert multiple rows.
- Understand relationships between tables.
- Retrieve records using SQL queries.
- Practice SQL Data Manipulation Language (DML).

---

# 📝 SQL Operations Performed

## Step 1 – Insert Data

Inserted sample records into:

- Doctors
- Patients
- Appointments
- Treatments
- MedicalRecords
- Billing

using SQL `INSERT INTO` statements.

---

## Step 2 – Retrieve First Record

Retrieved the first record from the first three tables.

### Doctors

```sql
SELECT *
FROM Doctors
WHERE DoctorID = 1;
```

### Patients

```sql
SELECT *
FROM Patients
WHERE PatientID = 1;
```

### Appointments

```sql
SELECT *
FROM Appointments
WHERE AppointmentID = 1;
```

---

# 📌 Sample Output

### Doctors

| DoctorID | Name | Specialization |
|----------|------|---------------|
| 1 | Dr. John Smith | Cardiology |

---

### Patients

| PatientID | Name | Gender |
|-----------|------|--------|
| 1 | Alice Johnson | Female |

---

### Appointments

| AppointmentID | PatientID | DoctorID | Status |
|--------------|-----------|----------|---------|
| 1 | 1 | 1 | Scheduled |

---

# 💡 SQL Concepts Used

- INSERT INTO
- SELECT
- WHERE Clause
- Primary Key
- Foreign Key
- Data Relationships
- SQL DML Commands

---

# 📚 Learning Outcomes

After completing this experiment, you will be able to:

- Insert records into SQL tables.
- Populate relational databases.
- Maintain table relationships.
- Retrieve specific records.
- Work with multiple related tables.
- Understand Hospital Management database structure.

---

# 🚀 How to Run

1. Create the Hospital Management database.
2. Create all required tables.
3. Execute the SQL `INSERT` statements.
4. Run the `SELECT` queries.
5. Verify the output.

---


# 🛠️ Technologies Used

- SQL
- Relational Database Management System (RDBMS)
- CodeChef SQL Intermediate

---

# 📖 Experiment Summary

This experiment focuses on populating a Hospital Management database using SQL. It demonstrates inserting records into multiple related tables and retrieving the first record from selected tables using SQL queries. The experiment strengthens understanding of SQL DML operations, relational database concepts, and table relationships through a real-world hospital database example.

---

## 👨‍💻 Author

**Ayush Bansal**

- B.E. Computer Science Engineering
- Chandigarh University

---

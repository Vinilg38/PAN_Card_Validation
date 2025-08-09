# PAN Card Validation

This project provides a solution for validating **Indian Permanent Account Numbers (PANs)** and includes a sample dataset and a database script.  
The purpose is to demonstrate a **data-driven approach** to checking the validity of PANs against a known dataset.

---

## 📂 Project Files

- **`PAN Number Validation - Problem Statement.pdf`**  
  A document outlining the problem and objectives of the project.

- **`PAN Number Validation Dataset.csv`**  
  A sample dataset containing PAN numbers and associated details for validation purposes.

- **`script.mssql`**  
  The SQL script for creating the necessary table to store the PAN data.

---

## 🚀 Getting Started

To use this project, you will need a SQL database (the provided script is for **PostgreSQL**, but it can be adapted for others).

1. **Set up the Database**  
   Execute the `CREATE TABLE` script provided below to create the `PAN_CARD_DATA` table.

2. **Import Data**  
   Import the data from **`PAN Number Validation Dataset.csv`** into the newly created `PAN_CARD_DATA` table.

3. **Run Your Validation Logic**  
   Use Python or SQL queries to validate new PAN numbers against the data in the table.

---

## 🗄 SQL CREATE TABLE Script

The following script will create a table named `PAN_CARD_DATA` with columns to store the PAN number, the holder's name, and the validation status.

```sql
CREATE TABLE PAN (
    pan_no TEXT
);

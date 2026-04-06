# CMSE 492 HW02 - SQL Mini-Project with Sakila

## Overview
This homework analyzes the Sakila database using SQL in a Jupyter notebook. The main focus of the project is to understand film category performance by examining rental activity, revenue, rankings, and category-level contribution to total revenue.

The notebook demonstrates several SQL concepts:
- multi-table joins
- grouped aggregation with HAVING
- common table expressions (CTEs)
- window functions
- query validation and sanity checks
- basic performance analysis with EXPLAIN
- manager-style reporting

## Files
- `HW02-STUDENT.ipynb` — fully executed notebook containing the analysis
- `docker-compose.yml` — Docker setup for the Sakila MySQL database and Adminer
- `README.md` — project overview and setup instructions

## Tools and Skills Demonstrated
This project showcases:
- SQL joins across multiple related tables
- aggregation and filtering with `GROUP BY` and `HAVING`
- multi-step SQL logic with CTEs
- ranking and percent-of-total analysis with window functions
- result validation through row-count checks and spot checks
- basic query-plan interpretation with `EXPLAIN`

## How to Run the Project

### 1. Clone the repository
```bash
git clone https://github.com/YOUR_USERNAME/cmse492-hw02-yourMSUNetID.git
cd cmse492-hw02-yourMSUNetID
```

### 2. Start the database and Adminer
```bash
docker compose up -d
```

This starts:

MySQL with the Sakila database on port 3306
Adminer on port 8080

### 3. Open Adminer (optional)

In local browser, go to:

http://localhost:8080

Typical connection values:
```bash
System: MySQL
Server: mysql
Username: root
Password: password
or the credentials expected by the provided image/documentation
Database: sakila
```

### 4. Open and run the notebook

Open HW02-STUDENT.ipynb in Jupyter or VS Code and run the notebook from top to bottom.
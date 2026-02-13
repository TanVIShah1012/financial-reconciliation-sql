Financial Reconciliation & Variance Detection System (SQL + Python)

Overview

This project simulates a month-end financial close and reconciliation workflow using SQL and Python.

A synthetic ledger database was generated programmatically to mimic real-world transactional systems. The project then applies SQL-based reconciliation logic, variance analysis, and anomaly detection techniques to identify discrepancies and unusual transaction behavior.

The goal is to demonstrate practical financial data engineering and analytical SQL skills in a realistic accounting workflow.

Technical Architecture

1️⃣ Synthetic Data Generation (Python)

Programmatically generated multi-month transactional ledger data

Simulated realistic financial behavior across:

Cash

Accounts Payable

Revenue

Salaries Expense

Bank Charges

Introduced controlled variance (~2%) to simulate reconciliation mismatches

2️⃣ SQL Reconciliation Workflow

Computed actual balances using aggregation queries

Compared against expected ERP balances

Calculated variance and variance %

Implemented drill-down reporting by batch and transaction

3️⃣ Advanced SQL Analytics

Common Table Expressions (CTEs)

Window functions (running balances)

Monthly rollups

Daily net flow with rolling aggregation

4️⃣ Anomaly Detection

Duplicate transaction detection

Z-score outlier detection per account

Suspicious reversal pattern detection

Revenue sign inconsistency checks

Key Outputs

finance.db — Synthetic financial database

Reconciliation summary report

Variance by account visualization

Running balance trend analysis

Daily net flow with rolling window

Audit-ready CSV exports for flagged anomalies

Example Insights

Variance analysis successfully identified accounts with simulated reconciliation gaps.

Window-function-based running balances revealed volatility patterns in cash activity.

Z-score anomaly detection flagged statistically extreme transactions.

Duplicate transaction checks demonstrated automated audit controls.

🚀 How to Reproduce (Colab / Python)

Run the synthetic data generator to create finance.db

Execute SQL reconciliation queries

Run anomaly detection and visualization cells

Export generated artifacts

All data used in this project is synthetic and locally generated.

Technologies Used

Python (sqlite3, pandas, numpy)

SQLite

SQL (CTEs, window functions, aggregation)

Matplotlib / Seaborn

Skills Demonstrated

Financial data modeling

Reconciliation logic implementation

Variance analysis

SQL analytics (intermediate–advanced)

Data anomaly detection

Synthetic data simulation

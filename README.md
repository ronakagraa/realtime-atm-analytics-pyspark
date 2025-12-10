ATM Big Data Analytics Project (PySpark)

This project demonstrates how PySpark can be used to process and analyze ATM sensor and transaction data at scale. It simulates real-world ATM behavior, detects anomalies such as fraud and overheating, and generates actionable insights.

The entire project runs on Google Colab, removing the need for any local installations such as Java, Spark, Hadoop, or winutils. This ensures a smooth, error-free experience across Windows, macOS, and Linux.

🧾 Project Summary

ATMs generate operational and transaction data continuously. This project processes that data using Big Data engineering techniques:

✔ Data Generation

Synthetic ATM data is created with:

ATM ID

Temperature

Cash levels (₹500 and ₹200 notes)

Transaction amount

Timestamp

✔ Data Processing (PySpark)

Using PySpark, the project performs:

RDD Operations: Basic transformations and filtering (e.g., count high-temperature events)

DataFrame Transformations: Add derived columns such as total_cash

Spark SQL: Fraud detection rules Temperature monitoring ATM performance summaries

✔ Output

Results are saved in organized CSV folders:

fraud_output/

temp_output/

cash_summary_output/

These files are lightweight and can be uploaded directly to GitHub.

💡 Why Use Google Colab for This Project?

Google Colab is the best platform for PySpark projects for beginners and students because:

⭐ 1. No Installation Needed

Local Spark setup often requires:

Java installation

Spark download

Hadoop/winutils configuration (Windows)

Environment variables

These typically cause errors like:

“Java not found” “No winutils.exe present” “Spark context failed to start”

Colab solves all of this automatically.

⭐ 2. Preconfigured Cloud Environment

Colab provides:

Cloud CPU

Enough memory for large datasets

Ability to run Spark smoothly

⭐ 3. Easy GitHub Integration

Colab allows direct saving to GitHub using:

File → Save a copy to GitHub

This makes it perfect for building portfolio-ready Big Data projects.

⭐ 4. Platform Independent

Works on:

Windows

macOS

Linux

Mobile (with restrictions)

No installation issues.

🏗️ Project Architecture (High Level) Data Generator → Raw ATM CSV → PySpark Engine │ ┌──────────── RDD Operations ────────────┐ │ │ High Temp Alerts Preprocessing │ │ └────────── DataFrames & SQL ─────────────┘ │ │ Fraud Detection Cash Summary │ │ CSV Outputs (GitHub-ready)

▶️ How to Run This Project (Google Colab)

Follow these simple steps:

Step 1 — Open Google Colab

Go to: https://colab.research.google.com

Click: New Notebook

Step 2 — Add Text and Code Cells

Paste the provided project notebook content:

Text → Markdown cells

Code → Code cells

Run cells one by one in order.

Step 3 — Generate Data

A synthetic ATM dataset is created (CSV).

Step 4 — Run the PySpark Pipeline

The notebook performs:

RDD operations

DataFrame transformations

Spark SQL queries

Step 5 — View and Download Results

Once executed, folders like:

fraud_output/

temp_output/

cash_summary_output/

will appear in the Colab file explorer.

You can download them for verification or include them in GitHub.

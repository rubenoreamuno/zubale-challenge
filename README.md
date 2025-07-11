# 🧠 Zubale Lead Data Engineer Assessment

This repository contains the solution to the Lead Data Engineer assessment provided by Zubale. It includes Python scripts, SQL queries, and documentation that solve a multi-part challenge involving CSV data transformation, PostgreSQL setup, and business insights extraction.

---

## 📦 Structure

```
.
├── data/                          # Original CSV files
├── scripts/                       # SQL scripts to create the tables
├── challenges/                    # The challenges notebooks
├── outputs/                       # Generated CSV outputs
│   ├── order_full_information.csv
│   ├── fixed_order_full_information.csv
│   └── kpi_product_orders/
|       ├── demanded-categories.csv
|       ├── demanded-products.csv
|       └── max-orders.csv
└── README.md                      # This file
```

---

## 🧩 Challenges Overview

### ✅ Challenge 1 – CSV Consolidation

Merged `orders.csv` and `products.csv` into `order_full_information.csv` with:
- `order_created_date`
- `order_id`
- `product_name`
- `quantity`
- `total_price`

### ✅ Challenge 2 – Currency Conversion

- Used `https://app.freecurrencyapi.com/` to convert BRL → USD
- Output: `fixed_order_full_information.csv`

### ✅ Challenge 3 – PostgreSQL Deployment

- Provisioned VM using GCP Compute Engine
- Set up PostgreSQL with Docker
- Loaded CSVs into tables via `COPY`
- Executed optimized SQL queries for:
  - Peak order date
  - Most demanded product
  - Top 3 most demanded categories

### ✅ Challenge 4 – Extended Analysis

Proposed additional KPIs:
- Purchase frequency per product
- Category seasonality
- Stockout risk index

Also proposed:
- ETL to BigQuery using Apache Airflow
- Optional ML pipeline for demand forecasting

---

## 🛠️ Technologies Used

- Python 3.10
- Pyspark
- PostgreSQL (via Docker)
- Google Cloud Platform
- SQL
- Markdown
- pandas

---

## 📧 Submission

Once completed, this repository is delivered to:

- 📤 Vladyslav Dodonov (vladyslav.dodonov@zubale.com)
- 📤 CC: Maria Bravo (maria.bravo@zubale.com )

---

## 📎 License

MIT — use freely with attribution.

# 🛠️ ETL & Data Warehousing Project: Apache Hop + Oracle Cloud

This project demonstrates the design and implementation of a complete ETL pipeline using **Apache Hop** and **Oracle Autonomous Data Warehouse**, integrated with **Tableau** for dashboard visualization. The goal was to simulate real-world data warehousing scenarios involving dimension and fact loading, slow-changing dimensions (SCDs), and end-to-end reporting.

---

## 📌 Project Highlights

- 🔄 **ETL Pipelines using Apache Hop**
  - Created robust workflows for loading `DimCustomer`, `DimProduct`, `FactSales`.
  - Implemented **SCD handling** using Dimension Lookup/Update node.
  - Used stream lookups for foreign key resolution and data cleansing.

- 🗄️ **Oracle Autonomous Data Warehouse**
  - Hosted star-schema data model with `DimDate`, `DimCustomer`, `DimProduct`, and `FactSales`.
  - Populated a full `DimDate` table (2016–2026) using dynamic SQL.
  - Ensured referential integrity and scalability.

- 📊 **Visualization using Tableau**
  - Built interactive dashboards for:
    - Employment vs. Unemployment rate trends (NYS data).
    - Category-wise sales analytics for "Guac Stop".
  - Connected securely to Oracle DB using Wallet config.

---

## 🧱 Data Model Overview

- **Star Schema**:
  - Fact Table: `FactSales`
  - Dimension Tables: `DimCustomer`, `DimProduct`, `DimDate`

> Refer to `sql/` folder for full schema and DDL scripts.

---

## ⚙️ ETL Pipelines

Apache Hop pipelines included:
- 📥 `LoadDimCustomer.hpl` – Direct load from Oracle.
- 🔁 `LoadDimProduct_SCD.hpl` – SCD Type-2 update from Excel.
- 📦 `LoadFactSales.hpl` – Complex load with stream lookups, filtering, and batch inserts.

---

## 📊 Dashboards

- **Employment Trends (NYS)**:
  - Monthly employment and insured unemployment rate forecasting.
- **Guac Stop Sales Insights**:
  - Category, brand, and product-level trends.
  - Yearly sales breakdown and product demand analysis.

> Find `.twb` files in `tableau_dashboards/`.

---

## 🔒 Secure Connectivity

- Configured using Oracle Wallet (`cwallet.sso`, `sqlnet.ora`, `tnsnames.ora`)
- JDBC connections for seamless interaction between Hop/Tableau and Oracle Cloud.

---

## 📁 Repository Content

| Folder | Description |
|--------|-------------|
| `sql/` | All DDL and sample data SQL scripts |
| `apache_hop_pipelines/` | Pipeline definitions (.hpl files) |
| `tableau_dashboards/` | Tableau visualization files |
| `architecture/` | ERD & ETL flow diagrams |
| `docs/` | Project proposal PDF and related documents |

---

## 📈 Future Improvements

- Automate ETL using Apache Hop workflows.
- Schedule pipelines via cron or Airflow.
- Integrate alerting and monitoring for ETL failures.
- Expand to Snowflake or Azure Synapse for scalability.

---

## 👨‍💻 Author

**Poorna Chandra Ramachandra**  
📫 [LinkedIn](https://linkedin.com/in/your-profile) | 🛠️ ETL, Data Warehousing, BI

---

## 📄 License

MIT License. See `LICENSE` file for details.


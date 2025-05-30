# 🛠️ ETL & Data Warehousing Project: Apache Hop + Oracle Cloud

This project demonstrates the design and implementation of a complete ETL pipeline using **Apache Hop** and **Oracle Autonomous Data Warehouse**, integrated with **Tableau** for dashboard visualization. The goal was to simulate real-world data warehousing scenarios involving dimension and fact loading, slow-changing dimensions (SCDs), and end-to-end reporting.

---

# 🛠️ ETL & Data Warehousing Project: Apache Hop + Oracle Cloud

This project demonstrates an end-to-end ETL implementation using **Apache Hop**, **Oracle Cloud Autonomous Data Warehouse**, and **Tableau** for reporting.

---

## 📌 Overview

- Created a star schema for the retail domain ("The Guac Stop").
- Built ETL pipelines in Apache Hop to load both dimension and fact tables.
- Integrated Tableau to develop interactive sales dashboards.
- Secure Oracle DB connectivity using Wallet config.

---

## 🧱 Entity Relationship Diagram (ERD)

![ERD](images/erd_model.png)

---

## 🧩 Data Warehouse Logical Model

This reflects the star schema design implemented on Oracle Cloud.

![Logical Model](images/logical_model.png)

---

## 🔄 ETL Pipeline in Apache Hop

ETL flow to load the `FACT_SALES` table with stream lookups, filters, and batch inserts.

![ETL Pipeline](images/etl_pipeline.png)

---

## 📊 Tableau Sales Dashboard

Interactive dashboard analyzing Category, Brand, and Product-wise sales performance.

![Tableau Dashboard](images/tableau_dashboard.png)

---

## 🧪 Technologies Used

- **ETL Tool**: Apache Hop
- **Data Warehouse**: Oracle Cloud ADW
- **Visualization**: Tableau
- **Languages**: SQL, PL/SQL

---

## ✅ Outcomes

- Developed practical ETL and data modeling skills.
- Automated dimension and fact table loads with stream lookups.
- Delivered insights via interactive Tableau dashboards.

---

## 👨‍💻 Author

**Poorna Chandra Ramachandra**  
🔗 [LinkedIn](https://linkedin.com/in/your-profile)  
📫 Reach out for collaboration or questions.

---

## 📄 License

MIT License. See `LICENSE` for usage rights.

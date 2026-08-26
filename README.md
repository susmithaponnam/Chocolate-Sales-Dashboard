# 🍫 Awesome Chocolates Sales Dashboard

An interactive **Power BI sales analytics dashboard** built to analyze the performance of Awesome Chocolates across sales, shipments, products, salespersons, profitability, and geography.

The dashboard transforms raw shipment data into an interactive business report with KPIs, trend analysis, product performance, salesperson comparisons, and geographic insights.

---

## 📊 Dashboard Preview


---

## 🎯 Project Overview

The goal of this project was to build a business-focused Power BI dashboard that provides a clear overview of sales and operational performance.

The dashboard allows users to explore:

* Overall sales/amount
* Shipment volume
* Boxes sold
* Total profit
* Profit percentage
* Current Year vs Previous Year performance
* Product performance
* Salesperson performance
* Geographic sales distribution
* Shipment size distribution

The report is designed to make it easy to move from **high-level KPIs to detailed business insights** through interactive visuals and filters.

---

## 🛠️ Tools & Technologies

* **Power BI Desktop** – Dashboard development and visualization
* **Microsoft Excel** – Source data
* **Power Query** – Data cleaning and transformation
* **DAX** – Measures and analytical calculations
* **Data Modeling** – Relationships between tables and dimensional analysis

---

## 📁 Dataset

The project uses the **Awesome Chocolates shipment dataset**, containing fictional business data related to chocolate shipments and sales.

The dataset includes information such as:

* Shipment dates
* Products
* Salespersons
* Geography
* Amount
* Boxes
* Profit

The data was provided as an Excel dataset as part of Chandoo's Power BI/Data Analytics learning resources.

[Data Source Link](https://github.com/chandoo-org/Power-BI/blob/main/Telugu%20Full%20Course/sample-chocolate-shipments-data-all-Apr-2025.xlsx)

## 🧹 Data Preparation

The raw Excel data was prepared using **Power Query** before building the report.

Key preparation steps included:

* Importing data from Excel
* Reviewing and correcting data types
* Cleaning and transforming columns
* Preparing date-related data
* Creating a calendar/date table
* Structuring the data for analysis
* Establishing relationships between tables

---

## 🧩 Data Model

The report uses a structured data model to connect shipment data with descriptive dimensions.

The main analytical areas include:

```text
                    Calendar
                       │
                       │
Product ──────── Shipments ──────── Salesperson
                       │
                       │
                   Geography
```

The shipment table contains the transactional data, while dimension tables provide additional context for analyzing the transactions.

This allows the same measures to be analyzed by different dimensions such as **time, product, salesperson, and geography**.

---

## 🧮 DAX Measures

DAX was used to create reusable measures for the dashboard rather than relying only on raw columns.

Some of the key calculations include:

* Total Amount
* Total Boxes
* Shipment Count
* Total Profit
* Profit %
* Previous Year Amount
* Current Year vs Previous Year
* 12-Month Performance
* Variance calculations

Example:

```DAX
Total Amount = SUM(shipments[Amount])
```

These measures dynamically respond to filters and selections made within the dashboard.

---

## 📈 Dashboard Features

### 1. KPI Overview

The top section provides a quick snapshot of the business through key performance indicators:

* **Amount**
* **Boxes**
* **Shipments**
* **Total Profit**
* **Profit %**

This gives users an immediate understanding of overall performance.

---

### 2. Amount — Current Year vs Previous Year

A line chart compares sales amount across the current and previous year.

This helps identify:

* Sales trends
* Growth and decline
* Seasonal patterns
* Changes in performance over time

---

### 3. Boxes — Current Year vs Previous Year

The dashboard also compares the number of boxes shipped across the current and previous year.

This provides an additional perspective on sales volume and shipment activity.

---

### 4. Amount by Geography

The geographic visualization shows how sales are distributed across different countries/regions.

This makes it easier to identify stronger and weaker markets.

---

### 5. Shipment Distribution

The shipment distribution chart visualizes shipment volumes based on the number of boxes in each shipment.

It provides an overview of shipment patterns and order sizes.

---

### 6. Top Products

The dashboard highlights the **Top 6 products based on sales amount**.

This allows users to quickly identify the products contributing most to overall revenue.

---

### 7. Top Salespersons

The **Top 6 Salespersons** section compares individual performance using metrics such as:

* Amount
* Boxes
* Profit %

This makes it easier to identify high-performing sales representatives.

---

### 8. Product Performance

The product table provides a detailed comparison of products based on:

* Product
* Amount
* Profit %

Conditional formatting is used to make differences in profitability easier to identify visually.

---

## 🎛️ Interactivity

The dashboard includes interactive Power BI features such as:

* Date filters
* Cross-filtering
* Interactive charts
* KPI cards
* Dynamic DAX measures
* Conditional formatting
* Interactive tables

Users can select different time periods, products, salespersons, or geographic categories and explore how the rest of the report responds.

---

## 📚 Key Skills Practiced

This project helped me strengthen my practical understanding of:

### Power BI

* Report and dashboard design
* Visual selection
* Interactive filtering
* KPI creation
* Data storytelling

### Power Query

* Data transformation
* Data cleaning
* Data type handling
* Preparing data for analysis

### DAX

* Measures
* Aggregations
* `SUM`
* `COUNT`
* `DISTINCTCOUNT`
* `CALCULATE`
* Time-based calculations
* Year-over-year analysis
* Variance calculations

### Data Modeling

* Fact and dimension tables
* Relationships
* Calendar tables
* Star-schema concepts

---

## 💡 Key Insights

The dashboard provides a consolidated view of the company's performance and makes it possible to explore questions such as:

* Which products generate the highest sales?
* Which salespersons contribute the most revenue?
* How is profitability distributed across products?
* How does current-year performance compare with the previous year?
* Which geographic markets contribute most to sales?
* What does the shipment-size distribution look like?
* How are sales and shipment volumes changing over time?

---

## 📂 Repository Structure

```text
Awesome-Chocolates-PowerBI/
│
├── README.md
├── Awesome_Chocolates_Dashboard.pbix
│
├── dataset/
│   └── awesome_chocolates.xlsx
│
└── images/
    └── dashboard-preview.png
```

> Update the filenames if your actual files use different names.

---

## 📌 Project Takeaway

This project gave me hands-on experience in taking a raw business dataset and turning it into an interactive analytical dashboard.

The complete workflow involved:

**Excel Data → Power Query → Data Model → DAX → Visualizations → Interactive Dashboard**

It helped me understand how data preparation, modeling, calculations, and visualization work together to create a useful business intelligence solution.

---

## 📚 Learning Resource & Dataset Credit

The project was developed while learning Power BI through **Chandoo's Data Analytics and Power BI resources**, using the Awesome Chocolates dataset provided through those resources.

The dashboard implementation, analysis, report layout, and learning outcomes presented here are part of my own practice and portfolio work.

**Learning resource:** [Chandoo.org](https://chandoo.org/)

---

## 👩‍💻 Author

**Susmitha Ponnam**

B.Tech — Computer Science & Engineering (AI)


---

⭐ *This project represents my hands-on practice in building end-to-end Power BI dashboards and applying data analytics concepts to a business dataset.*

# 📊 Sales Performance & Business Intelligence Dashboard

## 📌 Project Overview

This project was completed as part of a **Data Analysis Internship at Novexa Technologies**.

The project focuses on analyzing Superstore sales data to identify business trends, understand sales performance across different dimensions, and present the findings through **Python Exploratory Data Analysis (EDA)** and an interactive **Power BI dashboard**.

---

## 🎯 Project Objectives

* Analyze overall sales performance
* Identify high-performing product categories and sub-categories
* Analyze regional sales performance
* Identify sales trends over time
* Understand customer segment contribution
* Identify top-performing products and customers
* Analyze shipping performance
* Create an interactive business intelligence dashboard
* Generate meaningful business insights from the data

---

## 📂 Dataset Overview

The analysis uses the **Superstore Sales Dataset**.

| Attribute      | Details           |
| -------------- | ----------------- |
| Records        | 9,800             |
| Columns        | 18                |
| Time Period    | 2015–2018         |
| Duplicate Rows | 0                 |
| Missing Values | 11 in Postal Code |
| Profit Field   | Not available     |

Since the dataset does not contain a **Profit** column, the analysis focuses on sales performance, products, customers, regions, segments, order trends, and shipping performance.

---

## 🛠️ Tools & Technologies

* **Python**
* **Pandas**
* **Power BI**
* **DAX**
* **CSV / Excel**
* **Git & GitHub**

---

## 🔍 Exploratory Data Analysis

Python was used to perform data exploration and analysis, including:

* Dataset structure and data-quality checks
* Missing-value analysis
* Duplicate detection
* Date-range analysis
* Sales statistics
* Category and sub-category analysis
* Regional sales analysis
* Yearly and monthly sales trends
* Customer segment analysis
* Top customer analysis
* Top product analysis
* Shipping performance analysis
* Order and customer metrics

---

## 📊 Power BI Dashboard

The Power BI dashboard provides an interactive overview of Superstore sales performance.

### Key Performance Indicators

| KPI                     |         Value |
| ----------------------- | ------------: |
| Total Sales             | $2,261,536.78 |
| Total Orders            |         4,922 |
| Total Customers         |           793 |
| Average Shipping Days   |          3.96 |
| Average Sales per Order |       $459.48 |

### Dashboard Visualizations

The dashboard includes:

* 📈 Sales Trend Over Time
* 📊 Sales by Category
* 🌎 Sales by Region
* 👥 Sales by Customer Segment
* 🏆 Top 10 Products
* 🚚 Sales by Ship Mode
* 🔎 Interactive Year, Region, Category, and Segment slicers

---

## 💡 Key Business Insights

### Category Performance

Technology generated the highest sales among the three major categories, with approximately **$827,455.87** in sales.

### Regional Performance

The **West region** recorded the highest sales at approximately **$710,219.68**.

### Yearly Trend

Sales increased from approximately **$479,856.21 in 2015** to **$722,052.02 in 2018**.

### Customer Segments

The **Consumer segment** contributed approximately **$1.15 million** in sales, making it the largest segment by sales volume.

### Top Product

The **Canon imageCLASS 2200 Advanced Copier** generated approximately **$61,599.82**, the highest sales among the products analyzed.

### Monthly Performance

**November 2018** recorded the highest monthly sales at approximately **$117,938.16**.

### Shipping Performance

The overall average shipping time was approximately **3.96 days**.

---

## 🧮 DAX Measures

### Total Sales

```DAX
Total Sales =
SUM(superstore[Sales])
```

### Total Orders

```DAX
Total Orders =
DISTINCTCOUNT(superstore[Order ID])
```

### Total Customers

```DAX
Total Customers =
DISTINCTCOUNT(superstore[Customer ID])
```

### Shipping Days

A calculated column was created to determine the number of days between order and shipping:

```DAX
Shipping Days =
DATEDIFF(
    superstore[Order Date],
    superstore[Ship Date],
    DAY
)
```

### Average Shipping Days

```DAX
Avg Shipping Days =
AVERAGE(superstore[Shipping Days])
```

---

## 📁 Project Structure

```text
Sales-Performance-BI-Dashboard/
│
├── data/
│   └── superstore.csv
│
├── python/
│   └── EDA_script.py
│
├── powerbi/
│   └── Sales_and_Bi_dashboard.pbix
│
├── report/
│   └── Sales_Performance_Business_Intelligence_Report.docx
│
└── README.md
```

---

## 🔄 Project Workflow

```text
Raw Dataset
     ↓
Data Quality Checks
     ↓
Data Exploration & Cleaning
     ↓
Python EDA
     ↓
Business Insights
     ↓
Power BI Data Modeling
     ↓
DAX Measures & Calculations
     ↓
Interactive Dashboard
     ↓
Final Business Intelligence Report
```

---

## 📌 Project Outcome

This project demonstrates an end-to-end data analysis workflow, starting from raw sales data and progressing through exploratory analysis, business insight generation, data modeling, visualization, and dashboard development.

The final Power BI dashboard provides an interactive view of sales performance and allows users to explore the data using multiple filters.

---

## 👩‍💻 Author

**Harpreet Kaur**

**Data Analysis Internship Project**
**Novexa Technologies**

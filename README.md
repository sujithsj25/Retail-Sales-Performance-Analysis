# Retail Sales Performance Analysis

An end-to-end retail sales analytics project developed using **Microsoft Excel, Power Query, Pivot Tables, Power Pivot/Data Model, and DAX** to analyze sales, profitability, products, stores, customer segments, sales channels, and monthly performance.


## 📊 Dashboard Preview

![Retail Sales Performance Dashboard](./Version_1/Dashboard_Image/Retail_Sales_Performance_Dashboard.png)


## 📊 Project Overview

This project analyzes retail transaction data for the period **1 January 2025 to 31 December 2025**.

The objective is to transform raw retail datasets into a clean analytical model, calculate important business KPIs, and develop an interactive executive dashboard that can help management understand overall business performance and identify key areas of opportunity.

This is a **self-directed Data Analyst portfolio project** based on a realistic retail business scenario.

---

## 🎯 Business Objective

The analysis focuses on understanding:

- Overall sales and profitability
- Monthly sales performance
- Product and category performance
- Store performance
- Sales-channel performance
- Customer-segment performance
- Regional performance
- High-performing products and stores
- Profitability across different business dimensions

The final dashboard provides an interactive way to explore these areas using filters and visualizations.

---

## 📁 Project Structure

```text
Retail-Sales-Performance-Analysis/
│
├── README.md
├── PROJECT REQUIREMENTS.md
│
├── DataSets/
│   ├── customers.csv
│   ├── products.csv
│   ├── stores.csv
│   ├── orders.csv
│   └── order_items.csv
│
├── Resources/
│   └── icons/
│
├── Version_1/
│   ├── Retail_Sales_Performance_Dashboard.xlsx
│   └── Dashboard_Image/
│       └── Retail_Sales_Performance_Dashboard.png
│
└── .gitignore
```

---

## 📂 Dataset Description

The project uses five related datasets:

| Dataset | Description |
|---|---|
| `customers.csv` | Customer details and customer segments |
| `products.csv` | Product details, categories, prices and costs |
| `stores.csv` | Store and regional information |
| `orders.csv` | Order details including dates, customers, stores, channels, discounts and status |
| `order_items.csv` | Products and quantities associated with each order |

---

## 🧹 Data Cleaning & Preparation

The raw datasets were cleaned and transformed using **Power Query**.

The main preparation steps included:

- Handling duplicate customer records
- Standardizing text values and capitalization
- Handling missing and blank values
- Handling missing product prices
- Handling missing discount values
- Validating dates and quantities
- Checking order status values
- Standardizing customer-segment values
- Converting columns to appropriate data types
- Removing unnecessary fields where appropriate
- Preparing the datasets for analysis

Blank customer-segment values were handled and represented as **Unknown** rather than being removed from the analysis.

Power Query was used to make the data preparation process repeatable.

---

## 🗂️ Data Model

The cleaned datasets were connected through a relational data model.

```text
Customers
    │
    ▼
  Orders ─────────► Stores
    │
    ▼
Order Items ─────► Products
```

### Relationships

- Customers → Orders
- Stores → Orders
- Orders → Order Items
- Products → Order Items

This model allows the data to be analyzed across products, categories, stores, regions, customers, customer segments, sales channels and time.

---

## 📐 Key Metrics

The project uses calculated business metrics to evaluate sales and profitability.

### Gross Sales

```text
Gross Sales = Quantity × Unit Price
```

### Net Sales

```text
Net Sales = Gross Sales − Discount Amount
```

### Profit

```text
Profit = Net Sales − Product Cost
```

### Profit Margin

```text
Profit Margin % = Profit ÷ Net Sales × 100
```

### Average Order Value

```text
AOV = Net Sales ÷ Number of Orders
```

Other metrics include:

- Total Orders
- Units Sold
- Number of Customers
- Discount Amount
- Product Cost

---

## 📊 Dashboard

The project includes an interactive executive dashboard built in Excel.

### KPI Cards

- Net Sales
- Net Profit
- Profit Margin
- Total Orders
- Customers
- Average Order Value

### Dashboard Visualizations

- Top 10 Products by Net Sales
- Net Sales by Store
- Net Profit by Store
- Profit Margin by Store
- Monthly Net Sales Trend
- Net Sales by Category
- Profit by Category
- Sales by Channel
- Sales by Customer Segment

### Interactive Filters

The dashboard includes slicers for:

- Month
- Category
- Region
- Store
- Sales Channel
- Customer Segment

---

## 🔍 Key Business Insights

The analysis identified several important performance patterns.

### 1. Electronics is the leading category

Electronics is the strongest category in terms of net sales and is a major contributor to overall business revenue.

### 2. Ahmedabad Central Store is a strong-performing store

The store analysis identifies Ahmedabad Central Store among the highest-performing stores in terms of sales.

### 3. Electronics is the strongest profit contributor

Electronics also contributes significantly to overall profit, making it an important category for business performance.

### 4. Store is the leading sales channel

The Store channel generates the highest net sales, followed closely by the Website channel.

### 5. Smartphone 062 is a top-performing product

Smartphone 062 is one of the strongest products in the analysis and leads the Top 10 product analysis by net sales.

---

## 💡 Business Recommendations

Based on the dashboard analysis, the following actions can be considered:

### 1. Focus on high-performing Electronics products

Maintain sufficient inventory and targeted promotional strategies for high-performing Electronics products while monitoring their profitability.

### 2. Study high-performing stores

Investigate the factors contributing to strong store performance and identify practices that could potentially be applied to lower-performing stores.

### 3. Strengthen high-performing sales channels

Continue optimizing the Store and Website channels while investigating opportunities to improve the performance of lower-performing channels.

### 4. Monitor high-performing products

Use products such as Smartphone 062 for targeted promotions, cross-selling and inventory planning.

---

## 🛠️ Tools & Technologies

- **Microsoft Excel**
- **Power Query**
- **Pivot Tables**
- **Power Pivot / Data Model**
- **DAX**

---

## 📈 Skills Demonstrated

This project demonstrates practical experience in:

- Data cleaning
- Data transformation
- Data validation
- Data modeling
- Power Query
- Excel analytics
- Pivot Tables
- DAX calculations
- KPI development
- Business intelligence
- Dashboard development
- Data visualization
- Business analysis
- Insight generation
- Data-driven recommendations
- 

## 📋 Project Requirements

The original business assignment used for this project is available in:

**[PROJECT REQUIREMENTS.md](PROJECT%20REQUIREMENTS.md)**

It contains the business objective, datasets, required analysis, dashboard requirements and quality standards used to define the project scope.

---

## 🚀 Project Outcome

The project transformed multiple raw retail datasets into a structured analytical solution using Excel and Power Query.

The final dashboard enables users to interactively analyze:

**Sales → Profitability → Products → Stores → Categories → Channels → Customers → Monthly Performance**

The project demonstrates an end-to-end workflow from **raw data preparation to business insights and recommendations**.

---

## 👤 Project Type

**Self-Directed Data Analyst Portfolio Project**

**Industry:** Retail  
**Analysis Period:** 2025  
**Primary Tool:** Microsoft Excel# Retail-Sales-Performance-Analysis

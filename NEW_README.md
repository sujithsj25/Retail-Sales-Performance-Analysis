# Retail Sales Performance Dashboard

An interactive retail analytics dashboard created in **Microsoft Excel** to analyze sales, net profit, profit margin, products, stores, regions, customer segments, and sales channels for 2025.

![Retail Sales Performance Dashboard](Version_1/Dashboard%20Image/Dashboard.png)

## Project Overview

This self-directed Data Analyst portfolio project transforms retail transaction data for **1 January 2025 to 31 December 2025** into a clean analytical model and an executive dashboard.

The project demonstrates the complete analytics workflow:

```text
Data Cleaning → Data Modeling → KPI Calculation → Dashboard Design → Business Insights
```

## Business Objective

The dashboard helps management understand:

- Overall sales and profitability
- Monthly sales performance
- Product and category performance
- Store and regional performance
- Sales-channel performance
- Customer-segment performance
- High-performing products and stores
- Areas that may require business action

## Dashboard Features

### KPI Cards

- Net Sales
- Net Profit
- Profit Margin
- Total Orders
- Customers
- Average Order Value

### Visualizations

- Monthly Net Sales Trend
- Top 10 Products by Net Sales
- Net Sales by Category
- Profit by Category
- Net Sales and Profit by Store
- Profit Margin by Store
- Sales by Channel
- Sales by Customer Segment

### Interactive Slicers

The dashboard can be filtered by:

- Month
- Category
- Region
- Store
- Sales Channel
- Customer Segment

## Repository Structure

```text
Retail-Sales-Performance-Dashboard/
├── Data/
│   └── Retail_Analysis_Raw_Data.xlsx
├── Resorce/
├── Version_1/
│   ├── Dashboard/
│   │   └── Retail_Sales_Performance_Dashboard.xlsx
│   └── Dashboard Image/
│       └── Dashboard.png
├── PROJECT_REQUIREMENTS.md
├── README.md
└── NEW_README.md
```

## Source Data

| Dataset | Description |
|---|---|
| `customers.csv` | Customer details and customer segments |
| `products.csv` | Product details, categories, prices, and costs |
| `stores.csv` | Store and regional information |
| `orders.csv` | Order dates, customers, stores, channels, discounts, and status |
| `order_items.csv` | Products and quantities associated with each order |

## Data Preparation

The raw data was cleaned and transformed using **Power Query**.

Preparation included:

- Removing duplicate customer records
- Standardizing text and capitalization
- Handling missing and blank values
- Checking missing product prices and discounts
- Validating dates and quantities
- Checking order status values
- Standardizing customer segments
- Converting columns to suitable data types
- Preparing repeatable Power Query transformations

Blank customer segments were represented as **Unknown** instead of removing those records.

## Data Model

```text
Customers ─────► Orders ─────► Order Items ─────► Products
                    │
                    └────────► Stores
```

### Relationships

- Customers → Orders
- Stores → Orders
- Orders → Order Items
- Products → Order Items

## KPI Calculations

| Metric | Calculation |
|---|---|
| Gross Sales | Quantity × Unit Price |
| Discount Amount | Gross Sales × Discount Percentage |
| Net Sales | Gross Sales − Discount Amount |
| Product Cost | Quantity × Unit Cost |
| Profit | Net Sales − Product Cost |
| Profit Margin | Profit ÷ Net Sales × 100 |
| Average Order Value | Net Sales ÷ Number of Orders |

Other calculated measures include total orders, units sold, number of customers, and discount amount.

## Key Insights

- **Electronics** is the leading category by net sales and a major contributor to profit.
- **Ahmedabad Central Store** is one of the strongest-performing stores by sales.
- The **Store** channel generates the highest net sales, followed closely by the Website channel.
- **Smartphone 062** leads the Top 10 product analysis by net sales.

## Recommendations

1. Maintain sufficient inventory and targeted promotions for high-performing Electronics products while monitoring profitability.
2. Analyze successful practices at strong-performing stores and apply suitable improvements to weaker locations.
3. Continue optimizing the Store and Website channels while identifying opportunities in lower-performing channels.
4. Use top products such as Smartphone 062 for cross-selling, promotions, and inventory planning.
5. Review low-margin products and stores to identify pricing, cost, or sales opportunities.

## Tools and Skills

### Tools

- Microsoft Excel
- Power Query
- Pivot Tables
- Power Pivot and Excel Data Model
- DAX

### Skills Demonstrated

- Data cleaning
- Data transformation
- Data validation
- Data modeling
- KPI development
- Pivot Table analysis
- DAX calculations
- Dashboard development
- Data visualization
- Business analysis
- Insight generation

## How to Use the Dashboard

1. Open `Version_1/Dashboard/Retail_Sales_Performance_Dashboard.xlsx` in Microsoft Excel.
2. Enable editing if prompted.
3. Use the slicers to filter by month, category, region, store, channel, and customer segment.
4. Review KPI cards and visuals to compare sales and profitability across business dimensions.

## Project Requirements

The original project brief is available in [PROJECT_REQUIREMENTS.md](PROJECT_REQUIREMENTS.md).

## Project Details

- **Project type:** Self-directed Data Analyst portfolio project
- **Industry:** Retail
- **Analysis period:** 2025
- **Primary tool:** Microsoft Excel

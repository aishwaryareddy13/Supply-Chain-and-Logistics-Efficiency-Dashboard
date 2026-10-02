# Supply Chain & Logistics Efficiency Dashboard

An interactive **Supply Chain & Logistics Efficiency Dashboard** built with **Python** and **Streamlit** for analyzing supply chain operations, product performance, logistics costs, supplier performance, inventory movement, manufacturing efficiency, profitability, and operational KPIs.

The dashboard converts structured supply-chain datasets into interactive metrics and visual analytics so users can explore operational trends, identify inefficiencies, and support data-driven planning.

---

## Overview

Modern supply chains generate large volumes of operational data across products, suppliers, manufacturing, transportation, inventory, orders, and customer activity.

This project provides a centralized analytical dashboard for transforming that data into business insights.

The application supports:

- Supply chain KPI monitoring
- Product and category performance analysis
- Revenue and cost analysis
- Regional and demographic analysis
- Logistics and carrier analysis
- Supplier quality and lead-time analysis
- Manufacturing performance analysis
- Inventory and stock-turnover analysis
- Profitability and cost-efficiency analysis
- Interactive filtering and exploration
- Dataset upload and preprocessing
- CSV/Excel-oriented data workflows

The project is designed as a lightweight Streamlit analytics application that can run locally without Docker or a complex infrastructure setup.

---

## Project Objective

The primary objective of this project is to provide an interactive analytical platform that converts supply chain data into meaningful business insights.

The dashboard is designed to help users:

- Monitor supply chain performance
- Analyze operational KPIs
- Identify cost inefficiencies
- Evaluate supplier performance
- Analyze logistics and delivery timelines
- Understand inventory movement
- Compare product performance
- Analyze manufacturing efficiency
- Evaluate profitability
- Explore regional and demographic patterns
- Support data-driven operational planning

---

## Business Problem

Modern supply chains generate large volumes of operational data across:

- Products
- Suppliers
- Manufacturing
- Transportation
- Orders
- Inventory
- Delivery timelines
- Costs
- Revenue
- Customer activity

Traditional spreadsheet-based reporting can make it difficult to continuously analyze this information and identify operational inefficiencies.

Common challenges include:

- Inconsistent delivery times
- Increasing transportation costs
- Supplier performance variation
- Inventory inefficiencies
- Manufacturing cost variation
- Difficulty comparing product performance
- Limited visibility into profitability
- Manual data preparation and reporting

This project addresses these challenges by providing an interactive dashboard that converts supply chain data into visual and analytical insights.

---

## Key Features

### 1. Interactive Dashboard

The dashboard provides KPI cards, charts, tables, filters, and navigation for exploring supply chain performance from a single interface.

### 2. Data Loading & Preprocessing

- Load the default supply-chain dataset or upload a custom dataset
- Clean missing and inconsistent values
- Detect duplicates and data-quality issues
- Convert data types and normalize data where required
- Prepare processed data for analytics and visualization

### 3. Supply Chain KPIs

The dashboard includes KPIs such as:

- Total Revenue
- Average Manufacturing Cost
- Average Shipping Cost per Unit
- Profit Margin
- Stock Turnover Rate
- Total Cost
- Average Delivery / Lead Time
- Product and supplier counts
- Efficiency-related metrics

### 4. Revenue & Product Analysis

Analyze:

- Product sales by type
- Revenue by product type
- Revenue over lead times
- Revenue by location
- Revenue by customer demographics
- Product price distribution

### 5. Logistics & Operational Efficiency

Analyze:

- Lead Time vs. Order Quantity
- Shipping Costs by Carrier
- Manufacturing Lead Time vs. Manufacturing Cost
- Lead Time Efficiency by Supplier

### 6. Supplier & Quality Analysis

Analyze:

- Defect Rates by Supplier
- Defect Rate vs. Production Volume
- Manufacturing Cost per Unit by Product Type
- Manufacturing Lead Time by Supplier
- Supplier lead-time efficiency and variability

### 7. Inventory Analysis

The dashboard provides inventory-oriented views including:

- Days in Inventory by Product Type
- Stock Turnover Rate by Product Type
- Inventory movement
- Potential overstock indicators

Higher turnover indicates faster inventory movement, while lower turnover can highlight products requiring additional review.

### 8. Profitability & Cost Efficiency

The dashboard includes:

- Profit Margin by Product Type
- Price vs. Revenue analysis
- Cost vs. Revenue analysis
- Profit Margin vs. Price-to-Revenue analysis

These views help analyze pricing, cost structures, revenue contribution, and profitability patterns.

---

## Dashboard Analysis Areas

| Area | Analysis |
|---|---|
| **Home & Data Summary** | Dataset overview, data health, records, columns, statistics |
| **KPI Dashboard** | Revenue, costs, margins, turnover, and operational KPIs |
| **Revenue Analysis** | Product, location, demographic, and time-based revenue |
| **Product Analysis** | Sales volume, category performance, and pricing |
| **Logistics** | Lead times, order quantities, and carrier shipping costs |
| **Manufacturing** | Manufacturing costs, lead times, and production quality |
| **Supplier Performance** | Defect rates, lead times, and efficiency |
| **Customer Insights** | Demographic distribution and revenue contribution |
| **Profitability** | Margins, price/revenue, and cost/revenue relationships |
| **Inventory** | Days in inventory and stock turnover |
| **Reporting** | Filtered/processed data export workflows |

---

## Key Performance Indicators

| KPI | Description |
|---|---|
| **Total Revenue** | Total revenue generated from the available supply chain dataset |
| **Average Manufacturing Cost** | Average manufacturing cost across available records |
| **Average Shipping Cost per Unit** | Average transportation/shipping cost at unit level |
| **Profit Margin** | Profitability measure based on revenue and profit |
| **Stock Turnover Rate** | Indicator of inventory movement and turnover |
| **Total Cost** | Total cost associated with the analyzed supply chain records |
| **Average Lead Time** | Average delivery or lead-time measure |
| **Supplier Count** | Number of suppliers represented in the dataset |
| **Product Count** | Number of products represented in the dataset |

---

## Analytical Methods

The project uses the following analytical techniques:

- Descriptive statistics
- Mean
- Median
- Mode
- Standard deviation
- Correlation analysis
- Trend analysis
- IQR-based outlier detection
- Z-score-based outlier detection
- Data normalization
- Data transformation
- Pandas group-by operations
- Aggregation
- KPI computation

### Visualization Methods

The dashboard can use:

- Bar charts
- Line charts
- Scatter plots
- Histograms
- Pie charts
- Heatmaps
- KPI cards
- Tables

---

## System Architecture

The application follows a layered analytical architecture:

```text
┌──────────────────────────────┐
│        DATA SOURCES          │
│                              │
│   CSV / Excel / File Upload  │
└──────────────┬───────────────┘
               │
               ▼
┌──────────────────────────────┐
│    DATA PROCESSING LAYER     │
│                              │
│      Python / Pandas         │
│          NumPy               │
│                              │
│ Cleaning / Validation /      │
│ Transformation / Aggregation │
└──────────────┬───────────────┘
               │
               ▼
┌──────────────────────────────┐
│      ANALYTICAL LAYER        │
│                              │
│ Descriptive Statistics       │
│ Correlation Analysis         │
│ KPI Computation              │
│ Outlier Detection            │
└──────────────┬───────────────┘
               │
               ▼
┌──────────────────────────────┐
│    VISUALIZATION LAYER       │
│                              │
│ Matplotlib / Seaborn         │
│ Plotly / Streamlit           │
└──────────────┬───────────────┘
               │
               ▼
┌──────────────────────────────┐
│     INTERACTIVE DASHBOARD    │
│                              │
│ Filters / KPIs / Charts      │
│ Tables / Reports             │
└──────────────┬───────────────┘
               │
               ▼
┌──────────────────────────────┐
│     INSIGHTS & REPORTING     │
│                              │
│ Business Analysis /          │
│ Decision Support             │
└──────────────────────────────┘
```

---

## End-to-End Data Workflow

```text
Supply Chain Dataset
        │
        ▼
Data Ingestion
        │
        ▼
Data Validation
        │
        ▼
Data Cleaning
        │
        ├── Missing Values
        ├── Duplicate Records
        ├── Data Types
        └── Inconsistent Values
        │
        ▼
Data Transformation
        │
        ├── Normalization
        ├── Derived Metrics
        └── Aggregation
        │
        ▼
Statistical Analysis
        │
        ├── Descriptive Statistics
        ├── Correlation
        ├── Trend Analysis
        └── Outlier Detection
        │
        ▼
KPI Calculation
        │
        ▼
Visualization
        │
        ├── KPI Cards
        ├── Charts
        ├── Graphs
        └── Tables
        │
        ▼
Streamlit Dashboard
        │
        ▼
Interactive Filtering
        │
        ▼
Business Insights
```

---

## Data Loading & Preprocessing

The preprocessing workflow includes:

1. Load the dataset using Pandas.
2. Inspect dataset structure.
3. Validate data types.
4. Identify missing values.
5. Detect duplicate records.
6. Identify inconsistent values.
7. Convert fields to appropriate data types.
8. Normalize or transform required fields.
9. Detect potential outliers.
10. Prepare processed data for analysis.
11. Aggregate data for KPI calculations.
12. Pass processed data to visualization components.

---

## Dataset

The project uses structured supply-chain data in CSV format.

The documented project includes:

```text
supply_chain_data.csv
cleaned_supply_chain_data.csv
```

### Typical Dataset Fields

| Column | Description |
|---|---|
| `Product_ID` | Unique product identifier |
| `Product_Category` | Product category or segment |
| `Supplier` | Supplier/vendor |
| `Manufacturing_Cost` | Product manufacturing cost |
| `Transportation_Cost` | Shipment/transportation cost |
| `Order_Quantity` | Quantity ordered |
| `Lead_Time` | Time from order placement to delivery |
| `Revenue` | Sales revenue |
| `Profit` | Profit after expenses |
| `Region` | Geographic operating region |

---

## Project Structure

```text
Supply-Chain-Management-Dashboard/
│
├── main.py
├── supply_chain_dashboard.py
├── requirements.txt
│
├── supply_chain_data.csv
├── cleaned_supply_chain_data.csv
│
└── README.md
```

---

## Technology Stack

| Technology | Purpose |
|---|---|
| **Python 3.10** | Core programming environment |
| **Streamlit** | Interactive web dashboard |
| **Pandas** | Data loading, cleaning, transformation, and aggregation |
| **NumPy** | Numerical and mathematical operations |
| **Matplotlib** | Statistical and analytical visualizations |
| **Seaborn** | Statistical visualization and heatmaps |
| **Plotly** | Interactive visual analytics |
| **OpenPyXL** | Excel file integration |
| **CSV** | Primary dataset format |
| **Git/GitHub** | Version control and collaboration |

---

## Installation & Setup

### 1. Clone the Repository

```bash
git clone <your-repository-url>
cd Supply-Chain-Management-Dashboard
```

### 2. Check Python Version

```bash
python --version
```

### 3. Create a Virtual Environment

```bash
py -3.10 -m venv venv
```

### 4. Activate the Virtual Environment

Windows PowerShell:

```powershell
venv\Scripts\activate
```

### 5. Install Dependencies

```bash
pip install -r requirements.txt
```

### 6. Run the Dashboard

```bash
streamlit run supply_chain_dashboard.py
```

The application will be available at:

```text
http://localhost:8501
```

---

## Quick Start

```bash
git clone <your-repository-url>

cd Supply-Chain-Management-Dashboard

py -3.10 -m venv venv

venv\Scripts\activate

pip install -r requirements.txt

streamlit run supply_chain_dashboard.py
```

---

## Dashboard Pages

### Home

- Project overview
- Dataset information
- Basic metrics
- Dashboard navigation

### Data Summary

- Number of records
- Number of columns
- Data types
- Mean
- Median
- Standard deviation
- Missing values
- Duplicate records
- Data health

### KPI Dashboard

- Total Revenue
- Average Manufacturing Cost
- Average Shipping Cost per Unit
- Profit Margin
- Stock Turnover Rate
- Total Cost
- Average Lead Time

### Revenue & Product

- Revenue by Product Type
- Revenue over Lead Time
- Revenue by Location
- Revenue by Customer Demographics
- Price Distribution

### Logistics

- Lead Time vs. Order Quantity
- Shipping Costs by Carrier
- Manufacturing Lead Time vs. Manufacturing Cost
- Lead Time Efficiency by Supplier

### Supplier

- Defect Rates by Supplier
- Defect Rate vs. Production Volume
- Manufacturing Cost per Unit by Product Type
- Manufacturing Lead Time by Supplier

### Inventory

- Days in Inventory by Product Type
- Stock Turnover Rate by Product Type
- Inventory movement analysis

### Profitability & Cost

- Profit Margin by Product Type
- Price vs. Revenue
- Cost-to-Revenue Ratio by Product Type
- Profit Margin vs. Price-to-Revenue

---

## Business Use Cases

The dashboard can support:

- Supply chain performance monitoring
- Supplier performance review
- Logistics cost analysis
- Manufacturing efficiency analysis
- Inventory movement analysis
- Product profitability analysis
- Regional performance analysis
- Transportation and carrier analysis
- Quality and defect monitoring
- Operational bottleneck identification
- Management reporting and decision support

---

Add the appropriate project license here if one is defined for the repository.

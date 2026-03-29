# 👟 Adidas Interactive Sales Dashboard

An end-to-end interactive sales analytics dashboard built with **Python**, **Streamlit**, and **Plotly** — visualizing Adidas US retail performance across retailers, states, regions, and time.

![Python](https://img.shields.io/badge/Python-3.10+-blue?style=flat-square&logo=python)
![Streamlit](https://img.shields.io/badge/Streamlit-1.x-red?style=flat-square&logo=streamlit)
![Plotly](https://img.shields.io/badge/Plotly-Interactive-green?style=flat-square&logo=plotly)
![Pandas](https://img.shields.io/badge/Pandas-Data%20Analysis-150458?style=flat-square&logo=pandas)
![License](https://img.shields.io/badge/License-MIT-yellow?style=flat-square)

---

## 📊 Dashboard Preview

> *Multi-chart interactive dashboard with retailer sales, monthly trends, state-level breakdowns, and regional treemaps — all with live data export.*

---

## 🚀 Features

- **Retailer Sales Bar Chart** — Compare total sales across all Adidas retail partners
- **Monthly Sales Trend Line** — Track revenue performance over time
- **State-Level Dual-Axis Chart** — Total Sales (bar) + Units Sold (line) on a secondary Y-axis
- **Region & City Treemap** — Hierarchical breakdown of sales from Region → City level
- **CSV Export Buttons** — Download any chart's underlying data instantly
- **Expandable Data Tables** — View raw grouped data in-app with collapsible expanders

---

## 🗂️ Project Structure

```
adidas-sales-dashboard/
│
├── adidas_dashboard.py     # Main Streamlit app
├── Adidas.xlsx             # Source dataset
├── download.png            # Adidas logo image
├── requirements.txt        # Python dependencies
└── README.md               # Project documentation
```

---

## 🛠️ Tech Stack

| Tool | Purpose |
|------|---------|
| Python 3.10+ | Core language |
| Streamlit | Web app framework |
| Pandas | Data manipulation |
| Plotly Express | Interactive charts |
| Plotly Graph Objects | Custom dual-axis chart |
| openpyxl | Excel file reading |
| Pillow (PIL) | Logo image handling |

---

## ⚙️ Setup & Installation

### 1. Clone the Repository
```bash
git clone https://github.com/jayeshmachha/adidas-sales-dashboard.git
cd adidas-sales-dashboard
```

### 2. Install Dependencies
```bash
pip install -r requirements.txt
```

### 3. Run the App
```bash
streamlit run adidas_dashboard.py
```

The app will open in your browser at `http://localhost:8501`

---

---

## 📁 Dataset

The dataset (`Adidas.xlsx`) contains Adidas US sales records with the following key columns:

| Column | Description |
|--------|-------------|
| `Retailer` | Retail partner name |
| `InvoiceDate` | Date of transaction |
| `Region` | US sales region |
| `State` | US state |
| `City` | City of sale |
| `TotalSales` | Revenue generated ($) |
| `UnitsSold` | Number of units sold |

---

## 📈 Visualizations Breakdown

### 1. Total Sales by Retailer
Bar chart grouping revenue by retail partner — useful for identifying top-performing distribution channels.

### 2. Total Sales Over Time
Monthly line chart derived from `InvoiceDate` — highlights seasonal trends and revenue peaks.

### 3. Sales & Units Sold by State
Dual-axis combination chart (bar + line) allowing simultaneous comparison of revenue vs. volume sold per state.

### 4. Sales by Region & City (Treemap)
Hierarchical treemap breaking down total sales from region level down to individual cities — values formatted in Lakhs for readability.

---

## 💡 Key Learnings

- Built multi-chart Streamlit layouts using `st.columns()` for responsive design
- Used `plotly.graph_objects` for custom dual-axis charts
- Implemented dynamic CSV download buttons for each chart
- Applied `dt.strftime()` for clean Month-Year aggregation
- Formatted large numbers (Lakh-scale) for better readability in treemaps

---

## 🔗 Connect with Me

**Jayesh Machha**  
B.Tech — Artificial Intelligence & Data Science  
Dr. Babasaheb Ambedkar Technological University, Mumbai

[![LinkedIn](https://img.shields.io/badge/LinkedIn-Connect-blue?style=flat-square&logo=linkedin)](https://linkedin.com/in/jayesh-machha-166aa42b3)
[![GitHub](https://img.shields.io/badge/GitHub-Follow-black?style=flat-square&logo=github)](https://github.com/jayeshmachha)

---

## 📄 License

This project is licensed under the MIT License — feel free to use, modify, and distribute.

---

> *Built as part of my Data Analytics portfolio to demonstrate end-to-end dashboard development using Python and Streamlit.*

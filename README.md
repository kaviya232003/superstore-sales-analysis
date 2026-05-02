# 🛒 Superstore Sales Analysis

An exploratory data analysis (EDA) project on the Sample Superstore dataset using Python. Covers data cleaning, KPI calculation, and sales visualizations across regions, segments, and product categories.

---

## 📌 Project Overview

This project analyzes retail sales data from a US-based superstore to uncover trends in sales, profitability, and customer segments. The analysis includes data cleaning, key business metrics, and multiple chart visualizations built with Matplotlib and Seaborn.

---

## 📂 Dataset

- **File:** `Sample - Superstore_uncleaned data.xlsx`
- **Rows:** 9,999 orders
- **Columns:** 23 features including Order Date, Sales, Profit, Segment, Category, Region, and more

> ⚠️ The raw dataset contains dirty values (abbreviated region names, null values, inconsistent segment labels) which are cleaned as part of this project.

---

## 🧹 Data Cleaning Steps

| Issue | Fix Applied |
|---|---|
| Missing `Ship Mode` | Filled with `"unknown"` |
| Missing `Country` | Filled with `"United States"` |
| Missing `State` | Filled with `"unknown"` |
| `Region` values `'E'`, `'w'` | Replaced with `'East'`, `'West'` |
| `Segment` values `'HO'`, `'Cor'` | Replaced with `'Home Office'`, `'Corporate'` |

---

## 📊 KPIs Calculated

| Metric | Description |
|---|---|
| Total Sales | Sum of all sales revenue |
| Total Profit | Sum of all profit |
| Total Quantity | Total units ordered |
| Total Cost | Sum of cost price |
| Net Profit % | Average profit margin across orders |

---

## 📈 Visualizations

| Chart | Type | Insight |
|---|---|---|
| Monthly Sales Trend | Line chart | Seasonality patterns across months |
| Sales by Category | Donut chart | Furniture vs Office Supplies vs Technology |
| Sales by Sub-Category | Bar chart | Top-performing sub-categories |
| Top 10 States by Sales | Bar chart | Highest revenue states |
| Sales Share by Region | Pie chart | East / West / Central / South breakdown |
| Sales by Segment & Category | Grouped bar chart | Cross-analysis of segment and category |
| Key Metrics by Category | Styled table | Avg sales, total sales, item count, avg profit |

---

## 🛠️ Tech Stack

- **Python 3**
- **Pandas** — data manipulation and cleaning
- **NumPy** — numerical operations
- **Matplotlib** — base visualizations
- **Seaborn** — styled charts
- **Jupyter Notebook** — interactive analysis

---

## 🚀 Getting Started

### 1. Clone the repository

```bash
git clone https://github.com/your-username/superstore-analysis.git
cd superstore-analysis
```

### 2. Install dependencies

```bash
pip install pandas numpy matplotlib seaborn openpyxl jupyter
```

### 3. Add the dataset

Place the Excel file in the project folder and update the path in the notebook:

```python
data = pd.read_excel("Sample - Superstore_uncleaned data.xlsx")
```

### 4. Run the notebook

```bash
jupyter notebook finalproject.ipynb
```

---

## 📁 Project Structure

```
superstore-analysis/
│
├── finalproject.ipynb          # Main analysis notebook
├── Sample - Superstore_uncleaned data.xlsx  # Raw dataset
└── README.md                   # Project documentation
```

---

## 💡 Key Findings

- **Technology** is the highest revenue category
- **November and December** show peak sales — strong seasonal trend
- **California, New York, and Texas** are the top 3 states by revenue
- **West and East** regions dominate overall sales share
- Certain sub-categories show high sales but low profit margins

---

## 🙋 Author

Aathilakshmi kaviya
[GitHub](https://github.com/kaviya232003) · [LinkedIn]( https://www.linkedin.com/in/aathilakshmi-kaviya)

---

## 📄 License

This project is open source and available under the [MIT License](LICENSE).

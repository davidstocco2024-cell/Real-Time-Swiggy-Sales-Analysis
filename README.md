# 🍕 Real-Time Swiggy Sales Analysis

<div align="center">

![Python](https://img.shields.io/badge/Python-3.10+-3776AB?style=for-the-badge&logo=python&logoColor=white)
![Pandas](https://img.shields.io/badge/Pandas-150458?style=for-the-badge&logo=pandas&logoColor=white)
![Plotly](https://img.shields.io/badge/Plotly-3F4F75?style=for-the-badge&logo=plotly&logoColor=white)
![Seaborn](https://img.shields.io/badge/Seaborn-4C72B0?style=for-the-badge&logo=python&logoColor=white)
![Jupyter](https://img.shields.io/badge/Jupyter-F37626?style=for-the-badge&logo=jupyter&logoColor=white)

**End-to-end exploratory data analysis on Swiggy food delivery sales data.**  
Uncovering revenue trends, customer behavior, and geographic performance across India.

[📊 View Notebook](#) · [💼 LinkedIn](https://www.linkedin.com/in/david-stocco-35ba40278/) · [🐛 Report Issue](https://github.com/davidstocco2024-cell/Real-Time-Swiggy-Sales-Analysis/issues)

</div>

---

## 📌 Project Overview

This project performs a full exploratory data analysis (EDA) on Swiggy's food delivery sales dataset. The goal is to extract actionable business insights around revenue performance, customer ratings, food preferences, and geographic distribution — the kind of analysis that directly informs operational and marketing decisions for a food delivery platform.

---

## 🎯 Key Business Questions Answered

| # | Question | Method |
|---|----------|--------|
| 1 | What is the total and average revenue per order? | KPI aggregation |
| 2 | Which days of the week generate the most revenue? | Day-of-week groupby |
| 3 | Do customers prefer Veg or Non-Veg dishes? | Keyword classification + pie chart |
| 4 | Which states and cities drive the most sales? | Geographic groupby + horizontal bar |
| 5 | How does performance vary across quarters? | Period-based aggregation |
| 6 | What is the average customer rating? | Mean aggregation |

---

## 📊 KPIs Dashboard

| Metric | Description |
|--------|-------------|
| **Total Sales (INR)** | Sum of all order revenue |
| **Average Order Value** | Mean revenue per transaction |
| **Average Rating** | Customer satisfaction score |
| **Total Rating Count** | Volume of reviews received |
| **Total Orders** | Number of transactions analyzed |

---

## 📈 Visualizations

- **Daily Revenue Trend** — Bar chart showing revenue by day of week (Mon–Sun), highlighting peak sales days
- **Veg vs Non-Veg Revenue** — Donut chart comparing revenue contribution by food category
- **Revenue by State** — Horizontal bar chart ranking all states by total sales
- **Top 5 Cities by Sales** — Focused view on highest-performing cities
- **Quarterly Performance Summary** — Table with total sales, average rating and order count per quarter

---

## 🗂️ Project Structure

```
Real-Time-Swiggy-Sales-Analysis/
│
├── swiggy_sales.ipynb       # Main analysis notebook
├── swiggy_data.xlsx         # Source dataset (not included — see below)
└── README.md                # Project documentation
```

---

## ⚙️ Tech Stack

| Library | Purpose |
|---------|---------|
| `pandas` | Data loading, cleaning, transformation and aggregation |
| `numpy` | Numerical operations and conditional column creation |
| `matplotlib` | Base plotting layer |
| `seaborn` | Statistical chart styling |
| `plotly.express` | Interactive charts (pie, bar, geographic) |

---

## 🚀 Getting Started

### 1. Clone the repository
```bash
git clone https://github.com/davidstocco2024-cell/Real-Time-Swiggy-Sales-Analysis.git
cd Real-Time-Swiggy-Sales-Analysis
```

### 2. Install dependencies
```bash
pip install pandas numpy matplotlib seaborn plotly openpyxl
```

### 3. Add the dataset
Place `swiggy_data.xlsx` in the project root. Update the file path in cell 5 of the notebook:
```python
# Change this line to match your local path
df = pd.read_excel('swiggy_data.xlsx')
```

### 4. Run the notebook
```bash
jupyter notebook swiggy_sales.ipynb
```

---

## 💡 Key Insights

- **Food Category**: Revenue is classified into Veg/Non-Veg using keyword detection on dish names — a practical NLP-lite approach for uncleaned real-world data
- **Geographic Performance**: State and city-level breakdowns reveal which markets Swiggy dominates and which present growth opportunities
- **Day-of-Week Patterns**: Identifying peak revenue days helps optimize delivery staffing and promotional timing
- **Quarterly Trends**: Quarter-over-quarter comparison surfaces seasonality and growth trajectory

---

## 🔮 Next Steps

- [ ] Add monthly sales trend chart (time series line plot)
- [ ] Correlate ratings with revenue — do higher-rated restaurants earn more?
- [ ] Build an interactive Plotly dashboard combining all KPIs
- [ ] Add statistical testing to validate day-of-week revenue differences
- [ ] Connect to a SQL database for larger-scale querying (Python + SQL Server)

---

## 👤 Author

**David Stocco**  
Data Analyst | Python · SQL · Tableau  
📍 Mendoza, Argentina

[![LinkedIn](https://img.shields.io/badge/LinkedIn-Connect-0A66C2?style=flat&logo=linkedin)](https://www.linkedin.com/in/david-stocco-35ba40278/)
[![GitHub](https://img.shields.io/badge/GitHub-Follow-181717?style=flat&logo=github)](https://github.com/davidstocco2024-cell)

---

## 📄 License

This project is open source and available under the [MIT License](LICENSE).

---

<div align="center">
<sub>Built with 🐍 Python as part of a data analytics learning journey · 2026</sub>
</div>

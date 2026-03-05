# 🍕 Real-Time Swiggy Sales Analysis

<div align="center">

![Python](https://img.shields.io/badge/Python-3.10+-3776AB?style=for-the-badge&logo=python&logoColor=white)
![Pandas](https://img.shields.io/badge/Pandas-150458?style=for-the-badge&logo=pandas&logoColor=white)
![Plotly](https://img.shields.io/badge/Plotly-3F4F75?style=for-the-badge&logo=plotly&logoColor=white)
![Seaborn](https://img.shields.io/badge/Seaborn-4C72B0?style=for-the-badge&logo=python&logoColor=white)
![Jupyter](https://img.shields.io/badge/Jupyter-F37626?style=for-the-badge&logo=jupyter&logoColor=white)

**End-to-end exploratory data analysis on Swiggy food delivery sales data.**  
Uncovering revenue trends, customer behavior, and geographic performance across India.

[📊 View Notebook](./swiggy_sales.ipynb) · [💼 LinkedIn](https://www.linkedin.com/in/david-stocco-35ba40278/) · [🐛 Report Issue](https://github.com/davidstocco2024-cell/Real-Time-Swiggy-Sales-Analysis/issues)

</div>

---

## 📌 Project Overview

End-to-end exploratory data analysis on Swiggy's food delivery sales dataset covering **197,000+ orders** across multiple Indian states and cities. The goal is to extract actionable business insights around revenue performance, customer ratings, food preferences, and geographic distribution — the kind of analysis that directly informs operational and marketing decisions for a food delivery platform.

---

## 📊 Key KPIs

| Metric | Value |
|--------|-------|
| 💰 **Total Revenue** | ₹5,300,000+ |
| 🛒 **Total Orders** | 197,000+ |
| ⭐ **Average Rating** | Calculated per analysis |
| 🧾 **Average Order Value** | Derived from total sales |

---

## 📈 Visualizations

### 📅 Daily Revenue Trend (Mon–Sun)

> Revenue grouped by day of week to identify peak ordering days and staffing opportunities.

![Daily Sales Trend](./daily%20sales%20trend.png)

---

### 🥗 Revenue Contribution: Veg vs Non-Veg

> Dish names classified via keyword detection into Veg/Non-Veg categories to understand customer food preferences and revenue split.

![Revenue Contribution](./Revenue%20contribution.png)

---

### 🗺️ Revenue by State

> Horizontal bar chart ranking all states by total sales — identifies Swiggy's strongest and weakest markets geographically.

![Revenue by State](./Revenue%20by%20state.png)

---

### 🏙️ Top 5 Cities by Sales

> Focused view on the five highest-performing cities to guide market expansion and promotional investment decisions.

![Top 5 Cities](./Top%205%20cities.png)

---

## 🎯 Key Business Questions Answered

| # | Question | Method |
|---|----------|--------|
| 1 | What is the total and average revenue per order? | KPI aggregation |
| 2 | Which days of the week generate the most revenue? | Day-of-week `groupby` |
| 3 | Do customers prefer Veg or Non-Veg dishes? | Keyword classification + donut chart |
| 4 | Which states and cities drive the most sales? | Geographic `groupby` + horizontal bar |
| 5 | How does performance vary across quarters? | Period-based aggregation |
| 6 | What is the average customer rating? | Mean aggregation |

---

## ⚙️ Tech Stack

| Library | Purpose |
|---------|---------|
| `pandas` | Data loading, cleaning, transformation and aggregation |
| `numpy` | Numerical operations and conditional column creation (`np.where`) |
| `matplotlib` | Base plotting layer |
| `seaborn` | Statistical chart styling and whitegrid theme |
| `plotly.express` | Interactive charts — pie/donut, horizontal bar |

---

## 🗂️ Project Structure

```
Real-Time-Swiggy-Sales-Analysis/
│
├── swiggy_sales.ipynb          # Main analysis notebook
├── swiggy_data.xlsx            # Source dataset (not included — see setup)
├── daily sales trend.png       # Revenue by day of week
├── Revenue contribution.png    # Veg vs Non-Veg donut chart
├── Revenue by state.png        # Geographic revenue breakdown
├── Top 5 cities.png            # Top 5 cities by total sales
└── README.md                   # Project documentation
```

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
Place `swiggy_data.xlsx` in the project root, then update the path in the notebook:
```python
# Replace the hardcoded path with:
df = pd.read_excel('swiggy_data.xlsx')
```

### 4. Run the notebook
```bash
jupyter notebook swiggy_sales.ipynb
```

---

## 💡 Key Insights

- **Peak days**: Day-of-week analysis reveals which days concentrate the highest order volume — directly applicable for delivery capacity planning
- **Food preferences**: Keyword-based Veg/Non-Veg classification shows clear revenue dominance by category, guiding restaurant partnership strategy
- **Geographic concentration**: A small number of states and cities account for a disproportionate share of total revenue — typical power-law distribution in delivery markets
- **Quarterly trends**: Period-based aggregation surfaces seasonality patterns useful for demand forecasting

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

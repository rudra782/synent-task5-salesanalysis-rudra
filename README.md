# Superstore Sales Data Analysis

A data analysis project that explores business performance using the Superstore Sales Dataset. The analysis covers monthly revenue trends, top-selling products, profit analysis, and regional performance, culminating in a structured business insights report.

---

## Table of Contents

- [Project Overview](#project-overview)
- [Dataset](#dataset)
- [Objectives](#objectives)
- [Project Structure](#project-structure)
- [Technologies Used](#technologies-used)
- [Setup and Usage](#setup-and-usage)
- [Analysis Breakdown](#analysis-breakdown)
- [Key Findings](#key-findings)
- [Output](#output)
- [License](#license)

---

## Project Overview

This project performs end-to-end exploratory data analysis (EDA) on the Superstore Sales dataset using Python in Google Colab. The goal is to derive actionable business insights from transactional retail data by analyzing sales performance, profitability, customer segments, geographic distribution, and the impact of discounts.

---

## Dataset

**Name:** Superstore Sales Dataset  
**Source:** Public sample dataset (CSV format)  
**Records:** ~10,000 rows  
**Time Period:** 2014 - 2017  

**Key Columns:**

| Column | Description |
|---|---|
| Order ID | Unique order identifier |
| Order Date | Date the order was placed |
| Ship Date | Date the order was shipped |
| Ship Mode | Shipping method used |
| Customer ID | Unique customer identifier |
| Segment | Customer segment (Consumer, Corporate, Home Office) |
| Region | Geographic region |
| State | U.S. state of the customer |
| Category | Product category |
| Sub-Category | Product sub-category |
| Product Name | Name of the product |
| Sales | Revenue from the order |
| Quantity | Number of units sold |
| Discount | Discount applied |
| Profit | Profit from the order |

---

## Objectives

- Analyze monthly and yearly revenue trends
- Identify top-selling and most profitable products
- Examine profit performance by category, sub-category, and region
- Understand the impact of discounts on profit margins
- Evaluate customer segment and shipping mode performance
- Detect seasonal patterns and peak sales periods
- Identify loss-making products and areas of concern
- Generate a comprehensive business insights report

---

## Project Structure

```
superstore-sales-analysis/
│
├── Superstore_Sales_Analysis.ipynb   # Main Google Colab notebook
├── README.md                         # Project documentation
└── data/
    └── superstore.csv                # Dataset (or loaded via URL in notebook)
```

---

## Technologies Used

| Tool / Library | Purpose |
|---|---|
| Python 3.x | Core programming language |
| Pandas | Data manipulation and aggregation |
| NumPy | Numerical operations |
| Matplotlib | Static charts and visualizations |
| Seaborn | Statistical plots and heatmaps |
| Plotly | Interactive charts |
| Google Colab | Cloud-based notebook environment |

---

## Setup and Usage

### Option 1: Open in Google Colab (Recommended)

1. Open [Google Colab](https://colab.research.google.com/)
2. Upload the `Superstore_Sales_Analysis.ipynb` file or paste the cells manually
3. Run all cells in order from top to bottom
4. The dataset is automatically loaded from a public URL in Cell 3

### Option 2: Run Locally

1. Clone this repository:
   ```bash
   git clone https://github.com/rudra782/synent-task5-salesanalysis-rudra
   ```

2. Install the required libraries:
   ```bash
   pip install pandas numpy matplotlib seaborn plotly kaleido
   ```

3. Launch Jupyter Notebook:
   ```bash
   jupyter notebook Superstore_Sales_Analysis.ipynb
   ```

4. Run all cells in sequence

### Using Your Own Dataset

If you have your own Superstore CSV file, replace the URL line in Cell 3 with:

```python
df = pd.read_csv('your_file.csv', encoding='latin-1')
```

---

## Analysis Breakdown

The notebook is organized into 18 cells, each serving a specific purpose:

| Cell | Description |
|---|---|
| 1 | Install required libraries |
| 2 | Import all libraries and configure plot styles |
| 3 | Load dataset from URL or upload |
| 4 | Data overview and quality check |
| 5 | Feature engineering (Year, Month, Quarter, Profit Margin) |
| 6 | High-level KPI summary |
| 7 | Monthly revenue and profit trend line chart |
| 8 | Year-over-year revenue comparison |
| 9 | Top 10 products by revenue |
| 10 | Top 10 products by profit |
| 11 | Category and sub-category analysis |
| 12 | Customer segment and regional performance |
| 13 | Discount vs profit correlation and scatter plot |
| 14 | Seasonal sales heatmap |
| 15 | Top 10 loss-making products |
| 16 | Top 10 states by revenue and profit |
| 17 | Shipping mode performance analysis |
| 18 | Final business insights report (printed summary) |

---

## Key Findings

- Technology is the highest-revenue and most profitable product category
- Discounts above 20% consistently result in negative profit margins
- The West region leads in both revenue and profit across all years
- Q4 (October to December) shows the strongest seasonal sales spikes each year
- The Consumer segment accounts for approximately 50% of total sales
- Tables and Boosters in the Furniture category are among the top loss-making sub-categories
- Standard Class shipping is the most used and most profitable shipping mode
- Year-over-year revenue shows consistent growth from 2014 through 2017

---

## Output

The final cell of the notebook prints a formatted business insights report covering:

- Revenue and profit summary
- Monthly and seasonal trends
- Top and bottom performing products
- Customer segment analysis
- Regional performance
- Discount impact assessment
- Shipping mode insights
- Actionable business recommendations

---

## License

This project is licensed under the MIT License. You are free to use, modify, and distribute this code for personal or commercial purposes with attribution.

---

## Author

Developed as part of a data analysis task focused on business intelligence and retail sales performance.

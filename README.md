# E-Commerce Sales & Profitability Analysis

## Project Overview

This project analyzes the Superstore e-commerce dataset to evaluate sales performance, profitability, product performance, regional performance, and the relationship between discount levels and profit.

The project was developed as a portfolio project to demonstrate practical data analyst skills using Python and Jupyter Notebook.

## Table of Contents

- [Project Overview](#project-overview)
- [Business Questions](#business-questions)
- [Key Findings](#key-findings)
- [Project Structure](#project-structure)
- [Analysis Workflow](#analysis-workflow)
- [Tools & Technologies](#tools-and-technologies)
- [How to Run](#how-to-run)
- [Limitations](#limitations)

## Business Questions

This analysis focuses on the following questions:

1. How did sales and profit performance change over time?
2. Which product categories generated the most sales and profit?
3. Which sub-categories were the most and least profitable?
4. Which regions performed best in terms of sales and profitability?
5. Which products generated the highest sales?
6. Which products contributed the most to losses?
7. How were discount levels associated with profitability?

## Dataset

The dataset contains 9,994 transaction records from a Superstore e-commerce business.

Key columns include:

- Order Date
- Ship Date
- Ship Mode
- Customer
- Segment
- Region
- Category
- Sub-Category
- Product
- Sales
- Quantity
- Discount
- Profit

The original dataset was loaded using Windows-1252 encoding.

## Analysis Workflow

The analysis followed these steps:

1. Load the dataset.
2. Explore the dataset structure and quality.
3. Clean column names and convert date columns.
4. Create additional analytical features:
   - Year
   - Month
   - Month Name
   - Year-Month
   - Profit Margin
   - Shipping Days
5. Calculate key performance indicators.
6. Analyze yearly and monthly sales trends.
7. Analyze category performance.
8. Analyze sub-category profitability.
9. Analyze regional performance.
10. Analyze product performance.
11. Analyze the relationship between discount levels and profitability.
12. Summarize key business findings.

## Key Performance Indicators

| Metric | Value |
|---|---:|
| Total Sales | USD 2.297M |
| Total Profit | USD 286.397K |
| Profit Margin | 12.47% |
| Total Orders | 5,009 |
| Total Customers | 793 |
| Average Order Value | USD 458.61 |
| Average Shipping Time | 3.96 days |

## Key Findings

### Sales and Growth

- Sales generally increased over the four-year period.
- 2015 experienced a 2.83% decline in sales, while profit increased by 24.37%.
- 2016 recorded the strongest sales and profit growth.
- In 2017, sales continued to grow, but profit growth slowed.
- Profit margin declined from 13.43% in 2016 to 12.74% in 2017.

### Category Performance

- Technology generated the highest sales and achieved a profit margin of 17.40%.
- Office Supplies achieved a profit margin of 17.04%.
- Furniture generated approximately USD 742K in sales but had a profit margin of only 2.49%.
- Furniture represents the most significant profitability concern among the major categories.

### Sub-Category Performance

- Tables generated the largest loss at approximately USD -17.7K.
- Bookcases and Supplies also generated negative profit.
- Copiers were the strongest profit contributor, generating approximately USD 55.6K in profit.
- Phones and Accessories were also among the strongest profit contributors.

### Regional Performance

- West was the strongest overall region.
- West generated the highest sales, total profit, and profit margin.
- West generated approximately USD 725.5K in sales and USD 108.4K in profit.
- Central had the lowest profit margin at 7.92%.
- South generated the lowest sales but achieved a higher profit margin than Central.

### Discount and Profitability

- The 0% discount group recorded a 29.51% profit margin.
- The 20% discount group recorded an 11.82% profit margin.
- Aggregate profit became negative at the 30% discount level.
- Higher discount levels were strongly associated with lower profitability.
- The 70% and 80% discount groups recorded particularly severe negative profit margins.

This analysis is observational and does not establish that discounts alone caused negative profit.

## Visualizations

The project includes visualizations covering:

- Annual Sales and Profit Performance
- Annual Profit Margin
- Monthly Sales Trend
- Sales and Profit by Category
- Sub-Category Profitability
- Discount Level vs Profit Margin
- Regional Sales and Profit
- Top Products by Sales
- Products with the Lowest Profit

All visualizations are stored in the `visualization/` directory.

## Tools and Technologies

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Jupyter Notebook
- Git
- GitHub

## Project Structure

```text
ecommerce-sales-analysis/
│
├── data/
│   ├── superstore.csv
│   └── cleaned_superstore.csv
│
├── notebooks/
│   └── ecommerce_analysis_cleaned.ipynb
│
├── visualization/
│   ├── annual_sales_profit.png
│   ├── annual_profit_margin.png
│   ├── monthly_sales_trend.png
│   ├── category_sales_vs_profit.png
│   ├── subcategory_profitability.png
│   ├── discount_vs_profit_margin.png
│   ├── regional_sales_vs_profit.png
│   └── top_sales_vs_loss_making_products.png
│
├── README.md
├── requirements.txt
└── .gitignore
```

## How to Run

Clone the repository:

```bash
git clone YOUR_REPOSITORY_URL
cd ecommerce-sales-analysis
```

Install the required libraries:

```bash
pip install -r requirements.txt
```

Launch Jupyter Notebook:

```bash
jupyter notebook
```

Open:

```text
notebooks/ecommerce_analysis_cleaned.ipynb
```

Run the notebook from top to bottom.

## Limitations

This project focuses on descriptive and exploratory analysis.

The findings should not be interpreted as causal conclusions. For example, the observed relationship between higher discounts and lower profitability does not prove that discounts alone caused the losses.

Further analysis could investigate:

- Product-level discount strategies
- Discount by category and region
- Customer segment profitability
- Repeat customer behavior
- Shipping performance and profitability
- Statistical relationships between discount and profit

## Author

**Fathul**

Data Analyst Portfolio Project

# EDA on Retail Sales Data

**Track:** Data Analytics — OIBSIP (Oasis Infobyte Summer Internship Program)
**Task:** Level 1, Task 1 — EDA on Retail Sales Data

## Objective
Perform exploratory data analysis on a retail sales dataset to uncover patterns, customer
behaviour trends, and actionable business insights.

## Dataset
**Sample Superstore Dataset** (Kaggle) — 9,994 rows, 13 columns covering Ship Mode,
Customer Segment, Region, Category, Sub-Category, Sales, Quantity, Discount, and Profit.

> Note: This dataset does not include an Order Date column or customer age/gender fields.
> To stay faithful to the analytical intent of the task, this notebook substitutes:
> - **Ship Mode trend analysis** in place of a monthly/quarterly time series
> - **Customer Segment breakdown** in place of age/gender demographics

## Tools Used
- Python
- pandas
- matplotlib
- seaborn
- Jupyter Notebook

## Analysis Covered
1. Initial data inspection (shape, dtypes, nulls, duplicates)
2. Descriptive statistics
3. Ship Mode sales & profit analysis
4. Customer Segment breakdown
5. Product analysis (top sub-categories & category revenue)
6. Correlation heatmap
7. Discount vs Profit analysis
8. Business recommendations

## Key Findings
- Standard Class drives the highest sales volume but has the lowest average profit per order.
- The Consumer segment accounts for the majority of both orders and revenue.
- Discounts beyond 20% consistently push profit into negative territory, especially for Technology products.

## Files
- `EDA_Retail_Sales_Real.ipynb` — full analysis notebook
- `SampleSuperstore.csv` — dataset used

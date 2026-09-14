# Cleaning Data

**Track:** Data Analytics — OIBSIP (Oasis Infobyte Summer Internship Program)
**Task:** Level 1, Task 3 — Cleaning Data

## Objective
Take a deliberately messy retail sales dataset and systematically transform it into a
clean, analysis-ready dataset, documenting every decision made along the way.

## Dataset
**Retail Store Sales — Dirty for Data Cleaning** (Kaggle) — 12,575 rows, 11 columns.

## Tools Used
- Python
- pandas
- numpy
- scipy

## Cleaning Steps Performed
1. **Data quality report** — inspected shape, dtypes, nulls, and duplicates
2. **Missing value handling** — used the relationship `Total Spent = Quantity × Price Per Unit`
   to mathematically recover 609 missing Price Per Unit values exactly (rather than estimating).
   Remaining numeric gaps filled with column median. Missing `Item` values labeled
   "Unknown Item"; missing `Discount Applied` values labeled "Not Recorded" to avoid bias.
3. **Duplicate removal** — checked, 0 duplicates found
4. **Standardisation** — converted `Transaction Date` from text to datetime; corrected data types
5. **Outlier detection** — IQR method found 157 outliers in Total Spent (retained as
   legitimate high-value transactions), 0 in Price Per Unit or Quantity
6. **Before/after summary table**
7. **Saved cleaned dataset** to `retail_store_sales_cleaned.csv`

## Result
Original dataset: 12,575 rows with 6,629 total missing values across 5 columns.
Cleaned dataset: 12,575 rows, **0 missing values**, correct data types throughout.

## Files
- `Cleaning_Data.ipynb` — full cleaning notebook with documented decisions
- `retail_store_sales.csv` — original messy dataset
- `retail_store_sales_cleaned.csv` — final cleaned dataset

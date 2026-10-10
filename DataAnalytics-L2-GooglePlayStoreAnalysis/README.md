# Google Play Store Analysis (Data Analytics – Level 2)

An exploratory data analysis of Google Play Store apps and their user reviews, covering app categories, ratings, installs, pricing, app size, and review sentiment.

## Project Structure

```
DataAnalytics-L2-GooglePlayStoreAnalysis/
├── GooglePlayStoreAnalysis.ipynb      # Analysis notebook
├── googleplaystore.csv                # App metadata
├── googleplaystore_user_reviews.csv   # User reviews with sentiment labels
└── README.md
```

> Rename the notebook line above to match your actual `.ipynb` file name.

## Datasets

| File | Description | Rows (raw) |
|------|-------------|-----------|
| `googleplaystore.csv` | App name, category, rating, reviews, size, installs, type, price, content rating, genres, last updated, versions | 10,841 |
| `googleplaystore_user_reviews.csv` | Translated user reviews with sentiment label, polarity, and subjectivity | 64,295 |

## Data Cleaning

- Removed 483 duplicate rows and duplicate app names
- Stripped symbols (`+`, `,`, `$`) from **Installs** and **Price** and converted them to numeric
- Converted **Size** to megabytes (MB)
- Filled missing **Rating** values using the median rating of each **Category**

## Analysis Overview

- Distribution of apps across categories
- Ratings, installs, and reviews by category
- Free vs. paid apps and pricing patterns
- App size vs. ratings and installs
- Sentiment analysis of user reviews using the dataset's existing sentiment labels (no custom NLP scoring)

## Sentiment Summary

| Sentiment | Share of reviews |
|-----------|------------------|
| Positive | 64.1% |
| Negative | 20.8% |
| Neutral | 13.0% |

## Key Observations and Conclusion

The notebook contains 7 observations and a final conclusion, written from the outputs of the analysis. See the last sections of the notebook.

## How to Run

1. Download the notebook and both CSV files into the same folder.
2. Open the folder in VS Code.
3. Select a Python kernel (Python 3.9+ recommended).
4. Install the required libraries if needed:
   ```bash
   pip install pandas numpy matplotlib seaborn jupyter
   ```
5. Run all cells from top to bottom.

## Tools and Libraries

Python, Pandas, NumPy, Matplotlib, Seaborn, Jupyter Notebook

## Author

**Subhadeep Haldar**
BTech, Electronics and Communication Engineering, Meghnad Saha Institute of Technology, Kolkata

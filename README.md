# Customer Shopping Behavior Analysis

An end-to-end data analytics project that cleans customer shopping data with Python, explores the cleaned dataset through EDA, and presents shopping trends in an interactive Power BI dashboard.

![Power BI dashboard preview](images/dashboard_preview.png)

## Project workflow

1. **Data cleaning with Python** — inspect missing values and duplicates, standardize text/category labels, validate numeric ranges, and prepare a cleaned dataset using Pandas and NumPy.
2. **Exploratory Data Analysis (EDA)** — examine customer demographics, spending, product categories, payment methods, purchase frequency, and review ratings.
3. **Power BI dashboard** — summarize KPIs and visualize spending by category, payment-method distribution, customer counts by age group, top purchased items, and average ratings by category. Gender, season, and subscription status slicers support interactive exploration.

## Dashboard KPIs

- Total records: approximately **99.9K**
- Total spend: approximately **$5.98M**
- Average spend: **$59.88**
- Average review rating: **3.78**
- Average previous purchases: **25.39**

Values reflect the dashboard version included in this repository.

## Repository structure

```text
customer-shopping-behavior-analysis/
├── data/
│   ├── raw/customer_shopping_behavior.csv
│   └── processed/customer_shopping_behavior_cleaned.csv
├── images/dashboard_preview.png
├── notebooks/customer_shopping_behavior_analysis.ipynb
├── powerbi/customer_shopping_behavior_dashboard.pbix
├── requirements.txt
├── .gitignore
└── README.md
```

## Run the Python notebook

1. Install Python 3.10+ and Jupyter Notebook, or use VS Code with the Jupyter extension.
2. From the repository root, install dependencies:

   ```bash
   pip install -r requirements.txt
   ```

3. Open `notebooks/customer_shopping_behavior_analysis.ipynb`.
4. Run the notebook cells in order. The notebook reads the raw CSV from `data/raw/` and saves the cleaned CSV to `data/processed/`.

## Open the Power BI dashboard

Open `powerbi/customer_shopping_behavior_dashboard.pbix` in Microsoft Power BI Desktop. If Power BI prompts you to locate the source data, select `data/processed/customer_shopping_behavior_cleaned.csv` and update the source path as needed.

## Tools used

- Python, Pandas, NumPy
- Matplotlib, Seaborn (for EDA/visualization where used)
- Jupyter Notebook
- Microsoft Power BI and DAX

## Dataset

The project dataset contains customer purchase attributes such as age, gender, item, category, purchase amount, location, season, review rating, subscription status, payment method, and purchase frequency. The raw and cleaned CSV files are included to make the workflow reproducible.

## Notes

- This is a portfolio/learning project; insights are descriptive and should not be interpreted as causal findings.
- The `.pbix` file is a Power BI Desktop report, not a web-published dashboard. To view it, use Power BI Desktop.

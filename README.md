# Megaline Plan Revenue Analysis (Statistical Data Analysis)

This project analyzes customer behavior and revenue for two prepaid plans (Surf and Ultimate) offered by the telecom operator Megaline. The objective is to determine which plan generates higher revenue and provide insights to support marketing budget allocation.

## Business Question
Which prepaid plan (Surf or Ultimate) generates more revenue, and do revenue patterns differ by region (NY-NJ vs other areas)?

## Data
The analysis uses five datasets covering 500 customers and their 2018 activity:
- Users (demographics, city, plan, subscription/churn dates)
- Calls (call duration and dates)
- Messages (text counts and dates)
- Internet sessions (MB used and dates)
- Plans (pricing, included allowances, overage rates)

**Important billing rules**
- Call durations are rounded up to the next minute for each call.
- Monthly data usage is summed and then rounded up to the next GB (1024 MB).

## Key Steps
- Cleaned and validated data types, missing values, and inconsistencies
- Aggregated user usage by month:
  - Minutes used
  - Text messages sent
  - Data usage (GB per month)
- Calculated monthly revenue per user using plan allowances and overage pricing
- Performed exploratory data analysis:
  - Usage distributions (minutes, texts, data) by plan
  - Summary statistics (mean, variance, standard deviation)
  - Histograms and comparisons across plans
- Tested statistical hypotheses:
  1. Average revenue differs between Surf and Ultimate users
  2. Average revenue differs between NY-NJ users and users from other regions
  - Selected an appropriate alpha level and used hypothesis testing to support conclusions

## Tools
- Python
- pandas, NumPy
- SciPy (hypothesis testing)
- Matplotlib (visualization)

## Results Summary
- Identified usage and revenue patterns by plan
- Quantified differences in average revenue using statistical hypothesis tests
- Delivered plan recommendation insights to inform marketing spend allocation

## Files
- `notebook.ipynb` — full analysis in Jupyter Notebook
- `/datasets/` — source CSV files (if included locally)

## How to Run
1. Open the notebook in Jupyter / VS Code
2. Ensure datasets are available (update paths if needed)
3. Run all cells from top to bottom

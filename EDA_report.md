# Exploratory Data Analysis & Statistical Insights

## Dataset overview
- Records analyzed: 12,000
- Numeric variables analyzed: 8
- Duplicate records remaining: 0
- Missing values remaining: 0

## Descriptive statistics
The full descriptive-statistics table is provided in `eda_descriptive_statistics.csv`.
It includes count, mean, median, standard deviation, minimum, quartiles and maximum.

## Hypothesis 1 — Discount vs Profit Margin
**H0:** Discount rate and profit margin have no linear relationship.
**H1:** Higher discount rate is associated with lower profit margin.

Pearson correlation: **-0.595**
p-value: **0**
Conclusion at α=0.05: **Reject H0 — statistically significant relationship.**

## Hypothesis 2 — Quantity vs Sales Amount
**H0:** Quantity sold and sales amount have no linear relationship.
**H1:** Higher quantity sold is associated with higher sales amount.

Pearson correlation: **0.451**
p-value: **0**
Conclusion at α=0.05: **Reject H0 — statistically significant relationship.**

## Hypothesis 3 — Electronics vs Accessories Sales
**H0:** Mean sales amount is equal between Electronics and Accessories.
**H1:** Mean sales amount differs between Electronics and Accessories.

Electronics mean sales: **112,217.63**
Accessories mean sales: **5,679.70**
Welch t-test statistic: **74.044**
p-value: **0**
Conclusion at α=0.05: **Reject H0 — the category means differ significantly.**

## Top 5 critical findings
1. **Discounting and profitability:** Discount rate shows a negative correlation with profit margin (-0.595), indicating that discount policy should be monitored for margin impact.
2. **Volume and revenue:** Quantity and sales amount show a correlation of 0.451, indicating that sales volume is strongly connected to revenue generation.
3. **Category performance:** Electronics average sales per transaction are 19.76× the Accessories average.
4. **Profit distribution:** The profit histogram and box plot should be reviewed for skewness and extreme transactions before using averages for business decisions.
5. **Multivariate business view:** The discount-vs-profit scatter plot helps identify whether high-discount transactions cluster around weaker profitability and highlights potential pricing-policy outliers.

## Visualizations
- `eda_correlation_heatmap.png`
- `eda_hist_sales_amount.png`
- `eda_hist_profit.png`
- `eda_hist_profit_margin.png`
- `eda_box_sales_amount.png`
- `eda_box_profit.png`
- `eda_box_profit_margin.png`
- `eda_discount_vs_profit.png`
- `eda_sales_by_category.png`
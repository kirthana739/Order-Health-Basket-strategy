# Retail Sales Analysis

An end-to-end retail analytics portfolio project using Excel, Python, Google Colab, and Power BI. It explores eight related retail datasets, answers 21 assigned business questions, and adds independent analysis to investigate customer, product, order, store, and return patterns.

## Project overview

- **Business area:** retail sales performance and order health
- **Data:** eight CSV files covering customers, employees, orders, order items, products, returns, stores, and targets
- **Tools:** Microsoft Excel, Python, pandas, Google Colab, and Microsoft Power BI
- **Deliverables:** Excel analysis, Colab notebooks, analysis charts, a five-page Power BI report, and a custom Power BI theme

## Power BI dashboard

The Power BI report contains five pages:

1. **Executive Overview** — high-level retail sales performance
2. **Products & Employees** — product and employee performance
3. **Customers & Stores** — customer and store analysis
4. **Returns & Targets** — return patterns and target achievement
5. **Order Health & Basket Strategy** — order status, cancellations, regional exposure, sales channels, and product demand

The Order Health & Basket Strategy page includes KPI cards for total orders, cancellation rate, estimated cancelled value, average units per completed order, and completed profit margin. Its charts explore monthly cancellation rate, estimated cancelled value by region, order status by sales channel, average order value by sales channel, and top products by units sold.

> Estimated cancelled value is an estimate based on the order-item and product data. It should not be interpreted as actual completed revenue.

### Dashboard screenshots

#### Executive Overview

![Retail Sales Executive Overview](RETAIL%20SALES%20PERFORMANCE%20-%20Copy%20%282%29.png)

#### Products & Employees

![Products and Employee Performance](PRODUCTS%20AND%20EMPLOYEE%20PERFORMANCE.png)

#### Customers & Stores

![Customer and Store Performance](CUSTOMER%20AND%20STORE%20PERFORMANCE.png)

#### Returns & Targets

![Returns and Target Achievement](RETURNS%20AND%20TARGET%20ACHIEVEMENT.png)

The `.pbix` file is not currently listed in the repository. Add it if you want visitors to open and interact with the report in Power BI Desktop. Add a screenshot of the Order Health & Basket Strategy page after exporting its final design.

## Custom Power BI theme

The repository includes a light **Sage and Terracotta** theme, designed with a warm off-white canvas and muted green, terracotta, gold, and rose chart colors.

- **Theme file:** [`Retail_Sage_Terracotta_Theme.json`](Retail_Sage_Terracotta_Theme.json)
- **Apply it:** In Power BI Desktop, choose **Design → Import theme**, then select the JSON file.
- Individual formatting applied directly to a visual can take precedence over theme defaults. Recolor those visuals manually if needed.

## Excel analysis

The Excel workbook answers 21 assigned sales-performance questions. Topics include revenue, profit, quantity sold, monthly sales, regions, products, employees, customers, stores, sales channels, returns, and targets.

[Open the Excel workbook](Sales_Performance_Analysis.xlsx.xlsx)

## Python and Google Colab analysis

The Colab notebooks use pandas to explore the supplied CSV data and practise:

- Selecting and filtering data
- Cleaning and preprocessing
- Transforming and sorting
- Grouping and aggregation
- Combining datasets
- Date and string operations
- Statistical summaries

The independent analysis notebook also creates charts for additional business questions.

- [Pandas practice notebook](Pandas_Retail_Sales_Operations1.ipynb)
- [Independent questions notebook](Own_Questions_Retail_Sales_Analysis.ipynb)

To run a notebook in Google Colab, open it and upload the required CSV files when prompted. Keep the CSV column names unchanged unless you also update the notebook code.

## Independent analysis questions

These questions explore additional patterns in the supplied data. The repository includes a chart for each question.

1. **How does revenue vary by day of the week?** This can help identify busier and quieter shopping days.

   ![Revenue by day of the week](Revenue%20by%20day%20of%20the%20week.png)

2. **Do customer age groups prefer different product categories?** This compares units sold across age groups and categories.

   ![Units sold by age group and product category](Units%20sold%20by%20age%20group%20and%20product%20category.png)

3. **Which payment methods are used most, and which are associated with the most revenue?** This compares payment frequency and revenue.

   ![Orders and revenue by payment method](orders%20and%20revenue%20by%20payment%20method.png)

4. **Are larger discounts associated with more units sold?** This explores discount levels and item quantities.

   ![Discount level and quantity sold](Discount%20level%20and%20quantity%20sold.png)

5. **Which suppliers contribute the most revenue and profit?** This compares supplier-level sales and profit.

   ![Revenue and profit by supplier](Revenue%20and%20profit%20by%20supplier.png)

6. **How many days pass between a product launch and its first sale?** This explores how quickly products begin selling.

   ![Days from product launch to first sale](Days%20from%20product%20launch%20to%20first%20sale.png)

7. **Do long-time customers spend more than newer customers?** This compares signup timing with customer spending.

   ![Customer signup date and total spending](customer%20signup%20date%20and%20total%20spending.png)

8. **Which customer cities have the most orders and highest average order value?** This compares order volume and average order value by city.

   ![Order count and average order value by city](Order%20count%20and%20average%20order%20value%20by%20city.png)

9. **Are return reasons more common for particular product categories?** This checks how returns are distributed across categories and reasons.

   ![Returned items by category and reason](Returned%20items%20by%20category%20and%20reason.png)

10. **Is employee salary associated with revenue generated?** This explores a relationship in the supplied data; it does not show that salary causes revenue.

   ![Employee salary and revenue generated](Employee%20salary%20and%20revenue%20generated.png)

Charts show patterns in this dataset. They do not, by themselves, prove that one factor caused another.

## Data files

The project uses these eight CSV files:

- `customers.csv`
- `employees.csv`
- `order_items.csv`
- `orders.csv`
- `products.csv`
- `returns.csv`
- `stores.csv`
- `targets.csv`

Before sharing the repository publicly, confirm that customer and employee data are synthetic or approved for public release. Do not publish real customer email addresses, confidential salary information, or other personally identifiable or confidential data.

## Repository contents

```text
retail-sales-analysis/
├── README.md
├── Retail_Sage_Terracotta_Theme.json
├── Own_Questions_Retail_Sales_Analysis.ipynb
├── Pandas_Retail_Sales_Operations1.ipynb
├── Sales_Performance_Analysis.xlsx.xlsx
├── customers.csv
├── employees.csv
├── order_items.csv
├── orders.csv
├── products.csv
├── returns.csv
├── stores.csv
├── targets.csv
└── dashboard screenshots and analysis charts
```

## How to use

- Open the Excel workbook in Excel to review the analysis and summaries.
- Open either `.ipynb` notebook in Google Colab or Jupyter. In Colab, upload the required CSV files when prompted.
- To use the Power BI theme, import `Retail_Sage_Terracotta_Theme.json` from the **Design** tab in Power BI Desktop.
- View the dashboard screenshots above. If the `.pbix` file is added, open it in Power BI Desktop. When refreshing on another computer, update the data source paths as needed.

## Limitations

- Findings describe the supplied dataset and depend on the metric definitions used in each analysis.
- A relationship or correlation in a chart does not prove causation.
- The employee salary and revenue comparison is exploratory and should only be shared if the data is approved for that use.
- Confirm discount, sales, profit, return-rate, and target definitions before presenting them as official business metrics.

Retail Sales Analysis (2024)
This project looks at a year of retail sales data and finds out what's really going on in the business — which products sell best, which regions make the most money, and how sales change through the year.
The data isn't clean to start with. It has missing values, duplicate rows, messy text, and a few bad entries. Part of the project is cleaning that up before doing any analysis, just like you'd have to do with real data at a job.
What's in this project

data/sales_data.csv — the raw sales data (1,225 orders from 2024)
notebook/sales_analysis.ipynb — the main notebook with all the cleaning, analysis, and charts
images/ — the charts, saved as PNG files
generate_data.py — script that created the sample data
build_notebook.py — script that built the notebook
requirements.txt — list of Python packages needed

The data
Each row is one order, with these columns:
ColumnWhat it meansOrderIDID for the orderOrderDateDate the order was placedCategoryType of product (Electronics, Apparel, Home & Kitchen, Sports, Stationery)ProductName of the productRegionNorth, South, East, or WestCustomerSegmentConsumer, Small Business, or CorporateQuantityHow many units were soldUnitPricePrice per unitSalesTotal sale amountProfitProfit made on the order
How to run it
Install what you need:
bashpip install -r requirements.txt
Then open the notebook:
bashjupyter notebook notebook/sales_analysis.ipynb
If you want to start from scratch and regenerate everything:
bashpython generate_data.py
jupyter nbconvert --to notebook --execute --inplace notebook/sales_analysis.ipynb
Questions this project answers

Which categories and regions bring in the most sales and profit?
Do sales go up or down at certain times of year?
Which type of customer (Consumer, Small Business, Corporate) is most valuable?
Does selling more units mean more profit, or does margin matter more?

The answers, along with the reasoning, are in the notebook under "Key Insights" and "Recommendations" at the end.

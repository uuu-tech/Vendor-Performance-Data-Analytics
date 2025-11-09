### Vendor-Performance-Data-Analytics


This project is an end-to-end case study on vendor performance analytics.
The aim is to demonstrate how data can be extracted, transformed, analyzed, and finally presented in a 
meaningful way to help businesses make better decisions about their vendors.

The work combines SQL for data preparation, Python for analysis, and Power BI for dashboarding and reporting. 
The ultimate goal is to identify which vendors perform well, which ones underperform, and what insights 
can be drawn to improve procurement strategies and profitability.



## Project Components



1. Exploratory Data Analysis notebook contains the first steps of working with the dataset. 
   It focuses on cleaning, summarizing, and understanding data distributions.
2. Vendor Performance Analysis notebook builds on this and calculates performance metrics, 
   ranks vendors, and provides deeper insights into costs, deliveries, and sales.
3. SQL scripts prepare raw transactional data into clean summary tables for further analysis.
4. Power BI dashboards (if applicable) visualize the metrics and trends in an interactive format.


## Workflow



The work starts with extracting and cleaning raw data from multiple tables: purchases, sales, 
vendor invoices, and product prices. These are joined into a consolidated dataset.

Exploratory Data Analysis is then performed in Python. This includes basic statistics, detecting 
outliers, handling missing values, and plotting trends. It also highlights issues such as negative 
profit margins, unusually high freight costs, and products that sell much faster or slower than average.

The Vendor Performance Analysis extends this by computing KPIs such as gross profit, profit margin, 
freight costs, stock turnover, and correlations among variables. Vendors are compared and ranked, 
and recommendations are drawn for how businesses can improve vendor management.

Finally, Power BI dashboards provide a stakeholder-friendly view of the results.These dashboards 
allow interactive filtering, vendor scorecards, and visual summaries of performance.


## Key Insights



1. Some transactions show very large losses, with gross profit falling to around –52,000 in certain cases. 
   This highlights vendors or products that may not be profitable.
2. There are premium products with purchase prices as high as 7,500, much higher than the average, 
   which may need different pricing or marketing strategies.
3. Freight costs vary drastically from a few cents to over 250,000, which suggests inefficiencies in 
   logistics or inconsistent billing.
4. Stock turnover shows extreme variation, with some products selling out immediately while others never move.
5. Purchase quantity and sales quantity are almost perfectly correlated, which confirms that inventory 
   is generally well aligned with sales.
6. Higher sales prices are sometimes linked to lower profit margins, showing the effect of competitive 
   pricing pressure.


## Recommendations



1. Promote or adjust pricing for products that have high profit margins but low sales, to maximize value.
2. Investigate logistics costs and standardize freight to avoid extreme cost variations.
3. Reassess strategy for premium products with very high purchase prices.
4. Review underperforming vendors with consistent losses or delays, and consider alternative sourcing.


## Technologies Used



SQL for preparing and aggregating data.
Python (pandas, numpy, matplotlib, seaborn, plotly) for cleaning, exploration, and analysis.
Power BI for interactive dashboards.
Jupyter Notebooks for documenting the workflow.


## How to Run the Project



1. Load the raw dataset into a SQL database using the provided scripts.
2. Run the Exploratory Data Analysis notebook to understand the dataset.
3. Continue with the Vendor Performance Analysis notebook to compute KPIs and insights.

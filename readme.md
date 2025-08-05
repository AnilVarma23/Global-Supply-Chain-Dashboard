# Global Supply Chain Dashboard

## Overview
This repository contains the data and documentation for the Global Supply Chain Dashboard, a project that analyzes sales data for a fictional shipping company. 

->Dataset was loaded into the system from multiple sources

1. Sales Data - csv file directly from system
2. Inventory data - SQL connection using Big Query
3. SQL Queries

The dataset has been cleaned using Power Query, and visualizations have been created using Power BI to provide actionable insights into companies performance on various metrics.

## Data Loading Process
1. Sales data was loaded from a csv file from the system
2. Inventory data was loaded from BigQuery usng SQL connection, where SQL functions like window and group by were performed for basic understanding of the data.

## Data Cleaning Process
The raw Sales dataset was cleaned using Power query with the following steps:
- Removed duplicate entries to ensure data integrity.
- Handled missing values by either filling them with appropriate defaults or removing incomplete records.
- Standardized date formats for consistency.
- Corrected inconsistencies in categorical data (e.g., region names, payment modes).

## Visualization
The cleaned data was imported into Power BI to create an interactive Dashboard. Key visualizations include:
- **Margin %** : can be filtered by country, category, customer type
- **Order status** : Column chart to check the status of order and its value 
- **Customer type distribution** : Pie chart to check % of share
- **Profit Margin by Year** : Line chart to check the profit margin % over period of time

-> With the help of bookmark feature data can be filtered by Country and Category
- **Sales Revenue Distribution** : Bar chart used for understanding the distribution of revenue.
- **Profit Distribution** : Bar chart used for understanding the distribution of profit.
- **Added Dynamic slicer to chose between Revenue and Profit**

- **Presence in countries** : Based on order qty showcased country on the map

-> Shipping Timeline

-** Delivery status** : With the help of donut chart visibility of delivery status
-**Average Shipping Days** : Compared Planned vs actual avg shipping days based on shipping mode using clustered column chart
-**Orders by Shipping Mode** : Using column chart to check no of orders by shipping mode
-**Countrywise distribution of shipping status** : Check delivery staus based on country

Since this are all dynamic charts so we can select one of the metric and filter the data against it to understand the data better

-> Inventory
-**Avg Inventory** : Check average inventory of article category in line chart which can be filtered based on Region and category so as to understand trend over period of time

-> Scheduled Refresh and Incremental refresh
-**Auto refresh** : Auto refresh of Sales data of last 10 days which is to be run every day to provide daily updated dashboard to the stakeholders


## Usage
1. Open the Power BI file (`Global_Supply Chai Dashboard.pbix`) to explore the interactive dashboard.
2. Use the filters (Year, Region), bookmarks, navigation bar, dynamic slicers to analyze data.
3. Refer to the data folder for datasets.

## Requirements
- BigQuery excess for SQL query writing and analysis and connection to Power BI
- Power BI Desktop (for interacting with the dashboard).

## Contributing
Feel free to fork this repository and submit pull requests for improvements or additional analyses.

## License
This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## Acknowledgments
- Data source: Fictional Global Supply Chain dataset, Inventory dataset.
- Tools: BigQuery, Power BI.
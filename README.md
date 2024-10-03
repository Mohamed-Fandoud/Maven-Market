# Maven Market Dashboard

## Description
The Maven Market dashboard provides a comprehensive analysis of sales, profit, returns, and customer insights using two years of data from 1997 and 1998. The dashboard is designed to support weekly analysis, enabling stakeholders to explore key performance metrics across various dimensions, including products, customers, and stores. The data has been meticulously cleaned and prepared for analysis, with a focus on ensuring high data quality and accuracy.

### Key Features:
- **Two-Year Data Analysis**: Analyze data across 1997 and 1998, with weekly breakdowns of total transactions, revenue, profit, returns, and more.
- **ETL Process**: Data cleaning and transformation were performed using CSV imports, with transactions imported as a folder. Calendar elements like year, quarter, month, start of month, and start of the week were extracted to enable detailed analysis.
- **Customer Data Preparation**: The customer file was enhanced by merging first and last names into a full name column for identifying top customers. A conditional column was created to determine whether a customer is a parent, based on the presence of children.
- **Data Quality and Data Types**: All data files were thoroughly checked for column quality and data types before loading, ensuring accurate ETL processes.
- **Data Modeling**: A snowflake schema was implemented in the model view, connecting all relevant tables. A snapshot of this model is included in the dashboard.
- **Comprehensive Measures**: The following measures were created for detailed analysis:
  - Total Transactions
  - Total Revenue
  - Total Returns
  - Total Profit
  - Total Cost
  - Revenue Target
  - Revenue Per Customer
  - Return Rate
  - Quantity Sold
  - Quantity Returned
  - Profit Margin
  - Last Month's Transactions
  - Last Month's Revenue
  - Adjusted Profit
  - Last Month's Returns
  - Last Month's Profit
  - Average Retail Price
  - Adjusted Revenue
  - Adjusted Profit
  - Adjusted Price

### Dashboard Pages:
- **Overview Page**: Displays key metrics for the current month, including orders, profit, and revenue. It includes:
  - A **map per orders** using the country slicer.
  - A **treemap** to visualize orders by country.
  - A **weekly revenue chart** with a slider to navigate weekly data.
  - A **revenue vs. target chart** that calculates the target by adding 5% to the previous month’s revenue.
  
  ![Overview Snapshot](https://github.com/user-attachments/assets/2d69babe-c91b-4157-8751-92a34e8ad918)
  - **Product Page**: Features a numeric range slicer for adjusted price to show how profit changes with price variations. Line charts present profit, revenue, returns, and return rates for each product over two years.
  
  ![Product Snapshot](https://github.com/user-attachments/assets/93869d8d-d4b7-4f97-96cb-96aaaf586eb7)

- **Customer Page**: Provides insights into total customers and revenue per customer, using line charts for trend analysis over two years. A pie chart displays occupation distribution and the percentage of parent customers, with details on top customers.
  
  ![Customer Snapshot](https://github.com/user-attachments/assets/dc5dcc4e-b248-4393-8b31-18dd9432f782)

- **Stores Page**: Includes a decomposition tree allowing users to drill down by total transactions, country, state, city, and product brand. Each page also features space for snapshot views.
  
  ![Stores Snapshot](https://github.com/user-attachments/assets/54a2631b-3218-4410-b18e-ffd36e300204)

### Dynamic Features:
The dashboard is fully dynamic, allowing users to filter data and adjust views in real-time.

## Data Sources
- **Sales Data**: Transactional data from 1997 and 1998.
- **Customer Data**: Demographic and transactional information for customers.
- **Product Data**: Detailed product metrics for sales, returns, and profit margins.
- **Store Data**: Store-level performance data, including location-based filters.

All datasets were imported in CSV format, with the transaction data imported as a folder. Data was validated for quality, and ETL processes were applied before loading into the Power BI dashboard.

## Installation/Setup Instructions
1. Download and install [Power BI Desktop](https://powerbi.microsoft.com/desktop/).
2. Clone this repository or download the `.pbix` file.
3. Open the `MavenMarketDashboard.pbix` file in Power BI Desktop.
4. Make sure to link all data sources if necessary, especially if you're using dynamic or external datasets.

### Prerequisites:
- Power BI Desktop Version 2.95 or later is required.
- No additional libraries or plugins are needed for this dashboard.

## Usage Instructions
- **Overview Page**: Navigate key metrics with a drill-through to the product page, and use filters for specific product and brand analysis.
- **Product Page**: Adjust the numeric range slicer for adjusted price to see profit changes. Analyze product performance over the two years using line charts that display profit, revenue, returns, and return rate.
- **Customer Page**: Review customer trends using line charts for total customers and revenue per customer. The pie chart provides a breakdown of occupation and parent percentage, with details on top customers.
- **Stores Page**: Use the decomposition tree to explore total transactions, filtered by country, state, city, and product brand. This page also includes space for snapshot views for better visualization.

## Data Sources
- **Sales Data**: 
  - `MavenMarket_Returns_1997-1998.csv`: Data on returns for the years 1997 and 1998.
  - `MavenMarket_Transactions.csv`: Transactional data from the Maven Market.
- **Customer Data**: 
  - `MavenMarket_Customers.csv`: Demographic and transactional information for customers.
- **Product Data**: 
  - `MavenMarket_Products.csv`: Detailed product metrics for sales, returns, and profit margins.
- **Region Data**: 
  - `MavenMarket_Regions.csv`: Information on regions associated with the sales data.
- **Store Data**: 
  - `MavenMarket_Stores.csv`: Store-level performance data, including location-based filters.
- **Calendar Data**: 
  - `MavenMarket_Calendar.csv`: Calendar data used for time-based analysis.

- **Power BI Dashboard**:
  - `MavenMarket Dashboard.pbix`: The main Power BI dashboard file that presents the analysis and visualizations.

All datasets and the PBIX file are available in the `/datasets` folder of this repository.

## Installation/Setup Instructions
1. Download and install [Power BI Desktop](https://powerbi.microsoft.com/desktop/).
2. Clone this repository or download the `.pbix` file.
3. Open the `MavenMarket Dashboard.pbix` file in Power BI Desktop.
4. Make sure to link all data sources if necessary, especially if you're using dynamic or external datasets.



## Contact:
mohamedelsayedfandoud@gmail.com





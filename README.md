# Coffee Shop Sales - MY SQL + Power BI

## Project Overview

### 1. Project Objective:
- **Purpose**: This project aims to analyze the sales performance of a coffee shop. The goal is to track and understand sales trends over various time periods (e.g., day, month, year) and product categories.
- **Audience**: The target audience for this project is the management team, who will use the insights to make strategic decisions to enhance the coffee shop's sales and performance.
- **Key Deliverables**:
  - Analysis of sales across various time periods: day, month, year, hour, weekday, and weekend.
  - Insights into store locations and product categories.
  - Sales performance breakdown for different product types.

### 2. Data Sources:
- **Data Origin**: The sales data is contained in a CSV file.
- **Data Volume**: The dataset has 149,116 rows and 11 columns, providing detailed sales information to analyze trends and performance.

### 3. Key Metrics and KPIs:
- **Total Sales**: The overall revenue generated from sales.
- **Total Orders**: The total number of customer orders.
- **Total Quantity Sold**: The total number of products sold, helping to track product demand.

### 4. Visualizations and Reports:
- **Dashboards**: The project uses various visualization techniques:
  - Cards, donut charts, clustered bar charts, stacked bar charts, stacked column charts, and line charts.
  - Matrix cards for detailed breakdowns.
- **Filters and Interactions**: Includes slicers to filter data, actions linked to images for interactive elements, and tooltips for additional data display.
- **Page Layout**: A single-page layout is designed for presenting all sales performance insights in an easy-to-understand format.
![Coffee-shop-sales](https://github.com/user-attachments/assets/8fdae537-a5fc-4355-a436-ef981e05ddfe)

### 5. Data Analysis:
- **Transformations**: A new date table was created to match the foreign keys in the dataset, ensuring effective analysis over time.
- **Calculated Fields**: Extensive use of DAX functions for various calculations, including:
  - `SUM`, `FORMAT`, `SELECTEDVALUE`, `DISTINCTCOUNT`, `CALCULATE`, `TOTALMTD`, `DATEADD`, `CALENDAR`, `IF`, `AVERAGEX`, `ALLSELECTED`, `HOUR`, `DIVIDE`.

### 6. Challenges and Solutions:
- **Challenge 1: Difficulty calculating month-on-month growth differences**.
  - **Solution**: Implemented custom DAX measures to calculate MoM growth, ensuring accurate results even with missing or incomplete data.
- **Challenge 2: Adding title above the clustered bar chart along with total sales**.
  - **Solution**: Created a placeholder using a new measure and added it to the X-axis, then created a new measure for the title and added it to the data label.
- **Challenge 3: Ensuring accurate and meaningful insights in findings**.
  - **Solution**: Cross-verified with MySQL queries to validate the analysis.
  
## **Usage**
This dashboard provides management with tools to:
- Identify peak sales hours and days.
- Analyze store-level performance to identify top-performing locations.
- Monitor product demand and prioritize best-selling categories and products.
- Track overall sales trends and identify growth opportunities.

# Fetch-Data-from-a-live-source-and-Build-a-Power-BI-Dashboard
## Project Overview
This project focuses on analyzing Walmart sales data, including data fetching, processing, and visualization. The primary goal is to provide insights into sales trends and performance across different stores and departments using Power BI.
## Tools used
- Pandas
- Power BI (Power Query, Data Visualization)
## Tasks Performed
- The data was fetched from a CSV file hosted on GitHub. The data was read directly into a Pandas DataFrame using Python.
- Detected mixed date formats (dd-mm-yyyy and dd/mm/yyyy), Created a parsing function to handle both formats,Applied to Order Date and Ship Date columns, Formatted dates consistently as dd-mm-yyyy
- Save Processed CSV Locally

## Simple Walmart Sales Dashboard 
1. Import Your Processed Data
   - Open Power BI Desktop
   - Click "Get Data" → "Text/CSV" → Select your `"Walmart_processed.csv"`
   - Click "Load"
## 2. Create 4 Visuals Side-by-Side
   
## A. Top Row: Key Metrics (Cards)
   - Click the "Card" visual icon
   - Add these 2 cards:
       - Total Sales: Drag `Sales` to "Fields"
       - Total Profit:Drag `Profit` to "Fields"
## B. Middle Section: Filters (Slicers)
   - Click the "Slicer" visual icon.
   - Add these 2 slicers:
        - Category Filter: Drag `Category` field
        - Date Range: Drag `Order` Date field (set as date range)
## C. Bottom-Left: Sales Trend (Line Chart)
   - Click the "Line chart" icon
   - X-axis: `Order Date` (month/year)
   - Y-axis: `Sales`
## D. Bottom-Right: Profit by Category (Pie Chart)
   - Click the "Pie chart" icon
   - Legend: `Category`
   - Values: `Profit`

![Dashboard](https://github.com/Jayasenthur/Fetch-Data-from-a-live-source-and-Build-a-Power-BI-Dashboard/blob/main/SimpleDashboard.png)

# ecommerce-customer-behavior-analysis
E-Commerce sales dashboard using Excel and Power BI


## Project Overview
This project analyzes customer behavior and sales performance 
of a Brazilian e-commerce company (Olist) using Excel and Power BI.
The dataset contains 100,000+ real orders from 2016 to 2018.

---

## Tools Used
- Microsoft Excel — data cleaning and preparation
- Power BI Desktop — data modeling and dashboard

---

## Dataset
- Source: Olist Brazilian E-Commerce Dataset
- Link: https://www.kaggle.com/datasets/olistbr/brazilian-ecommerce
- Size: 90,000+ orders across 8 CSV files
- Period: January 2016 to December 2018

---

## What I Did

### Excel
- Imported 4 CSV files into Excel
- Cleaned data — removed duplicates, blank rows, cancelled orders
- Fixed date formats across all columns
- Combined tables using VLOOKUP
- Created Master Sheet as olist_data with all required columns

### Power BI
- Imported cleaned Excel file into Power BI
- Loaded 3 additional tables — Products, Order Items, Payments
- Created data model by building relationships between tables
- Built DAX measures for key metrics
- Designed interactive dashboard with 6 visuals

---

## DAX Measures Created
```
Total Revenue = SUM('Olist_Data'[price])
Total Orders = DISTINCTCOUNT('Olist_Data'[order_id])
Avg Order Value = DIVIDE([Total Revenue],[Total Orders])

```

---

## Dashboard Visuals
| Visual | Description |
|--------|-------------|
| KPI Cards | Total Revenue, Orders, Avg Order Value, Customers |
| Line Chart | Monthly revenue trend 2016-2018 |
| Bar Chart | Top 5 product categories by revenue |
| Bar Chart | Top 5 states by number of orders |
| Donut Chart | Payment method split |
| Year Slicer | Filter all visuals by 2016, 2017, 2018 |

---

## Dashboard Preview
!<img width="882" height="491" alt="image" src="https://github.com/user-attachments/assets/abd156c1-44d4-43dd-8a82-ec501690c568" />


---

## Key Insights Found
1. Total revenue grew by Year
2. Beleza_saude and relogios_presents is the top selling category with 1.4M revenue
3. Sao Paulo generates 42% of all orders in Brazil
4. Credit card is the most used payment method at 74%


---

## Project Structure
```
ecommerce-customer-behavior-analysis/
│
├── Ecommerce_Project.xlsx      # Cleaned master data file
├── Ecommerce_Dashboard.pbix    # Power BI dashboard
├── dashboard_screenshot.png    # Dashboard image
└── README.md                   # Project documentation
```

---

## How to Use
1. Download the dataset from Kaggle link above
2. Open Ecommerce_Project.xlsx to see cleaned data
3. Open Ecommerce_Dashboard.pbix in Power BI Desktop
4. Use the year slicer to filter by 2016, 2017 or 2018


---

## Skills Demonstrated
- Data Cleaning and Preparation
- VLOOKUP and Excel Formulas
- Power BI Data Modeling
- DAX Measures and Calculations
- Dashboard Design
- Business Insights and Analysis

---

## Author
Name: Akash Babra
Tool: Excel + Power BI
Dataset: Olist Brazilian E-Commerce (Kaggle)
```

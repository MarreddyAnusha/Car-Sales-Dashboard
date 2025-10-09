# Car Sales Dashboard - Power BI Project

## About Company
Our company, a car dealership, aims to enhance sales performance tracking and analysis through an efficient Car Sales Dashboard in Power BI.

## Objective
Design and develop a dynamic, interactive Car Sales Dashboard to visualize critical KPIs, enabling data-driven decision-making and understanding sales performance trends over time.

## Problem Statement 1: KPI’s Requirement
### Sales Overview:
- Year-to-Date (YTD) Total Sales
- Month-to-Date (MTD) Total Sales
- Year-over-Year (YOY) Growth in Total Sales
- Difference between YTD Sales and Previous Year-to-Date (PTYD) Sales

### Average Price Analysis:
- YTD Average Price
- MTD Average Price
- YOY Growth in Average Price
- Difference between YTD Average Price and PTYD Average Price

### Cars Sold Metrics:
- YTD Cars Sold
- MTD Cars Sold
- YOY Growth in Cars Sold
- Difference between YTD Cars Sold and PTYD Cars Sold

## Problem Statement 2: Charts Requirement
1. **YTD Sales Weekly Trend:** Display a line chart illustrating the weekly trend of YTD sales. The X-axis should represent weeks, and the Y-axis should show the total sales amount.
2. **YTD Total Sales by Body Style:** Visualize the distribution of YTD total sales across different car body styles using a Pie chart.
3. **YTD Total Sales by Color:** Present the contribution of various car colors to the YTD total sales through a pie chart.
4. **YTD Cars Sold by Dealer Region:** Showcase the YTD sales data based on different dealer regions using a map chart to visualize the sales distribution geographically.
5. **Company-Wise Sales Trend in Grid Form:** Provide a tabular grid that displays the sales trend for each company. The grid should showcase the company name along with their YTD sales figures.
6. **Details Grid Showing All Car Sales Information:** Create a detailed grid that presents all relevant information for each car sale, including car model, body style, color, sales amount, dealer region, date, etc.

## Data Available
### Car Data:
- Car ID
- Date
- Customer Name
- Gender
- Annual Income
- Dealer Name
- Company
- Model
- Engine
- Transmission
- Color
- Price ($)
- Dealer No
- Body Style
- Phone
- Dealer Region

### Calendar Table (Created):
- Date
- Month
- Week
- Year

### DashBoard 
<img width="1297" height="734" alt="Screenshot 2025-10-10 003329" src="https://github.com/user-attachments/assets/0234b7ba-381b-46fd-93a8-c496c4d7e91d" />


<img width="1290" height="730" alt="Screenshot 2025-10-10 003435" src="https://github.com/user-attachments/assets/1111449b-a915-493b-ac32-2cf6b9d11b34" />



**Problem Statement 1: KPI’s**

**Sales Overview:**
- **YTD Total Sales:** $371.2M
    - **Formula:** `SUM('Car Data'[Total Sales])`
- **MTD Total Sales:** $54.28M
    - **Formula:** `CALCULATE(SUM('Car Data'[Total Sales]), DATESMTD('Calendar Table'[Date]))`
- **YOY Growth in Total Sales:** 23.6%
    - **Formula:** `[Sales Difference]/[PTYD Total Sales]`
- **Difference between YTD Sales and PTYD Sales:** $70.8M
    - **Formula:** `[YTD Car Sales]-[PTYD Car Sales]`

**Average Price Analysis:**
- **YTD Average Price:** $28.0k
    - **Formula:** `TOTALYTD([Avg Price],'Calendar Table'[Date])`
- **MTD Average Price:** $28.26k
    - **Formula:** `TOTALMTD([Avg Price],'Calendar Table'[Date])`
- **YOY Growth in Average Price:** -0.79%
    - **Formula:** `[Avg Price Diff]/[PTYD Avg Price]`
- **Difference between YTD Average Price and PTYD Average Price:** $0.22k loss
    - **Formula:** `[YTD Avg Price]-[PTYD Avg Price]`

**Cars Sold Metrics:**
- **YTD Cars Sold:** 13.3K
    - **Formula:** `SUM('Car Data'[YTD Car Solds])`
- **MTD Cars Sold:** 1.92k
    - **Formula:** `CALCULATE(SUM('Car Data'[MTD Cars Sold]), DATESMTD('Calendar Table'[Date]))`
- **YOY Growth in

 Cars Sold:** 19.73%
    - **Formula:** `car_data[Cars Sold Diff]/[YTD Car Solds]`
- **Difference between YTD Cars Sold and PTYD Cars Sold:** 3K
    - **Formula:** `[YTD Car Solds]-[PTYD Car Solds]`
 
**Problem Statement 2: Charts**


**YTD Sales Weekly Trend:**
<img width="809" height="442" alt="Screenshot 2025-10-10 003529" src="https://github.com/user-attachments/assets/91315de8-cce1-4dfd-9ab7-9821a2caa635" />



**YTD Total Sales by Body Style:**
<img width="505" height="435" alt="Screenshot 2025-10-10 003629" src="https://github.com/user-attachments/assets/68a0f38d-2a46-4435-8ca5-bd8f28c639b1" />


**YTD Total Sales by Color:** 
<img width="493" height="420" alt="Screenshot 2025-10-10 003718" src="https://github.com/user-attachments/assets/4e6ccaf9-ffc8-4b9e-bbdb-09b77c6f09b5" />


**YTD Cars Sold by Dealer Region:** 
<img width="809" height="442" alt="Screenshot 2025-10-10 003801" src="https://github.com/user-attachments/assets/cf2e10b0-3819-4321-a5a9-91b5e57f7cc2" />



**Company-Wise Sales Trend in Grid Form:** 
<img width="1038" height="438" alt="Screenshot 2025-10-10 003915" src="https://github.com/user-attachments/assets/b856bd3c-e0f4-4c81-9bbb-95b9b288a65c" />




**Details Grid Showing All Car Sales Information:** 
<img width="1299" height="673" alt="Screenshot 2025-10-10 004005" src="https://github.com/user-attachments/assets/09c33180-84e4-4d0c-b527-551381baa933" />

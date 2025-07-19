# Ankit Ecommerce Sales Dashboard
![logo](https://github.com/codeSavvy-ln/Power-BI/blob/6e9bbf99ca732d203a88f9b4abd4274fa901c90f/Ankit%20Ecommerce%20Sales%20Dashboard%20Project/Ankit%20Ecommerce%20Sales%20Dashboard%20SS.png)

## **Project Overview**

This project demonstrates an interactive dashboard created on Power BI to track the sales of an ecommerce shop.


## **ETL Pipeline Breakdown**

### **1. Data Extraction**
- **Weather Data:** Extracted both **Details**, and **Orders** data into power BI. 
- **Air Quality Data:** Collected using the AirVisual API, which provides air quality measurements such as PM2.5, PM10, and AQI (Air Quality Index).
  
### **2. Data Transformation**
- **Created a new column test** with value of combining these 2 columns = Amount * Quantity
- **Designed and implemented data models** by establishing relationships between Order and Details tables with 1 to 1 relation and joining by order id column which is common in both.
- **Changed the data type** of order date column in orders table from text to date. 
- Convert temperature units (Kelvin to Celsius).
- Merge weather and air quality datasets based on date and location.
- Create additional features such as "Feels like temperature" or AQI categories (Good, Moderate, Unhealthy, etc.).

### **3. Data Loading**
- Store the cleaned and transformed data into a PostgreSQL database.
- Database schema includes separate tables for **weather**, **air quality**, and **merged data**.
  
--------------------------------------------------------------------------------------------------------
**CHART NAME**                 |   **CHART TYPE**   |**Data in x-axis/Legend**|  **Data in y-axis/Value**
-------------------------------|--------------------|-------------------------|--------------------------
Profit by Month                |   Stack Column     |  Order Date (Month)     | Sum of Profit
Sum of Profit by Sub-Ctegory   |   Stack Bar Graph  |  Sum of Profit          | Subcategory        
Sum of Amount by State         |   Stack Bar Graph  |  Sum of Profit          | State
Sum of Amount by CustomerName  |   Stacked Column   |  CustomerName           | Sum of Amount
Sum of Quality by category     |   Donut Chart      |  Category               | Sum of Quantity
Sum of Quantity by PaymentMode |   Donut Chart      |  PaymentMode            | Sum of Quantity



### **Prerequisites to run the Project**
- **Power BI** 
- **Source Data** [Details.csv](https://github.com/codeSavvy-ln/Power-BI/blob/main/Ankit%20Ecommerce%20Sales%20Dashboard%20Project/Details.csv) and [Orders.csv](https://github.com/codeSavvy-ln/Power-BI/blob/main/Ankit%20Ecommerce%20Sales%20Dashboard%20Project/Orders.csv)
- **Gradient Color Backgroud**
    -  ![Dark Gradient Background Color](https://github.com/codeSavvy-ln/Power-BI/blob/main/Ankit%20Ecommerce%20Sales%20Dashboard%20Project/dark-gradient%20background.jpg)

# Ankit Ecommerce Sales Dashboard
![logo](https://github.com/codeSavvy-ln/Power-BI/blob/6e9bbf99ca732d203a88f9b4abd4274fa901c90f/Ankit%20Ecommerce%20Sales%20Dashboard%20Project/Ankit%20Ecommerce%20Sales%20Dashboard%20SS.png)

## **Project Overview**

This project demonstrates an interactive dashboard created on Power BI to track the sales of an ecommerce shop.

### **Prerequisites to Create the Project**
- **Power BI** 
- **Source Data** [Details.csv](https://github.com/codeSavvy-ln/Power-BI/blob/main/Ankit%20Ecommerce%20Sales%20Dashboard%20Project/Details.csv) and [Orders.csv](https://github.com/codeSavvy-ln/Power-BI/blob/main/Ankit%20Ecommerce%20Sales%20Dashboard%20Project/Orders.csv)
- **Gradient Color Backgroud** [Dark Gradient Background Color](https://github.com/codeSavvy-ln/Power-BI/blob/main/Ankit%20Ecommerce%20Sales%20Dashboard%20Project/dark-gradient%20background.jpg)


## **IMPLEMENTATION OF DASHBORAD ON POWER BI**

### **1. Data Extraction**
- **Extracted data** from both **Details**, and **Orders** table into power BI to visualize it after cleaning and transforming it.
- 

### **2. Data Transformation**
- **Created a new column AOV** with value of combining these 2 columns = Amount/Quantity. Data type should be whole numbers.
    - This column will be used in **Sum of AOV(Avergae Order Value)** chart.
- **Designed and implemented data models** by establishing relationships between Order and Details tables with 1 to 1 relation and joining by order id column which is common in both.
- **Changed the data type** of order date column in orders table from text to date. 

### **3. Data Visualization**
All the types of charts and the column or value used inside them for visualization is mentioned below: 
  
--------------------------------------------------------------------------------------------------------
**CHART NAME**                 | **CHART TYPE**     |**Data in x-axis/Legend**|  **Data in y-axis/Value**
-------------------------------|--------------------|-------------------------|--------------------------
Profit by Month                |   Stack Column     |  Order Date (Month)     | Sum of Profit
Sum of Profit by Sub-Ctegory   |   Stack Bar Graph  |  Sum of Profit          | Subcategory        
Sum of Amount by State         |   Stack Bar Graph  |  Sum of Profit          | State
Sum of Amount by CustomerName  |   Stacked Column   |  CustomerName           | Sum of Amount
Sum of Quality by category     |   Donut Chart      |  Category               | Sum of Quantity
Sum of Quantity by PaymentMode |   Donut Chart      |  PaymentMode            | Sum of Quantity

**Implemented Few More Visualizations:**
- Cards
  - Sum of Amount
  - Sum of Quantity
  - Sum of AOV (Average Order Value)
  - Sum of Profit

- Filters
    - Quaters: It will filter data for any of the 4 Quaters.
    - State: It will filter data for each state.
 

### **How to run this Project**
Download and open this file into your Power BI tool - [Ankit Ecommerce Sales Dashboard](https://github.com/codeSavvy-ln/Power-BI/blob/main/Ankit%20Ecommerce%20Sales%20Dashboard%20Project/Ankit%20Ecommerce%20Sales%20Dshboard.pbix) 

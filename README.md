# 📊 Customer Insights Dashboard (Power BI)

A full-featured analytics dashboard built in **Power BI** to demonstrate skills in data modeling, DAX, interactive visual design, and business analytics.  
The project includes a clean **Star Schema**, advanced KPIs, time intelligence, and drillthrough navigation.

---

## 📁 Project Overview

This dashboard provides insights into customer behavior, lifetime value distribution, segmentation performance, and revenue dynamics across multiple regions and product categories.

The solution includes:

- A structured **Star Schema** data model  
- Advanced **DAX measures** (Time Intelligence, CALCULATE, SWITCH, SELECTEDVALUE)  
- Interactive KPI cards  
- Metric selector with dynamic switching  
- Segmentation into High / Medium / Low value customers  
- Top 10 customers by LTV  
- Dedicated **Drillthrough page** with detailed customer info  
- A custom **Modern Minimal theme (JSON)** for professional design  

---

## 🧩 Tech Stack

- **Power BI Desktop (2023+)**
- **Power Query**
- **DAX**
- **JSON Theme**
- **Data modeling (Star Schema)**

---

## 📂 Repository Structure

Customer_Insights_Dashboard.pbix  
README.md  

data/  
  sales_and_customer_insights.csv  

screenshots/  
  overview.jpg  
  insights.jpg  
  star-schema.jpg  

theme/  
  modern_minimal.json  

---

## 🧱 Data Model (Star Schema)

### FACT_Sales
- Transaction_ID  
- Customer_ID  
- Product_ID  
- Region  
- Purchase_Frequency  
- Average_Order_Value  
- Time_Between_Purchases  
- Preferred_Purchase_Times  

### DIM_CUSTOMER
- Customer_ID  
- Region  
- Lifetime_Value  
- Customer Segment (Low / Medium / High)

### DIM_PRODUCT
- Product_ID  
- Most_Frequent_Category  
- Launch_Date  
- Peak_Sales_Date  
- Season

### DIM_REGION
- Region

### DIM_Date
- Date  
- Year  
- MonthNumber  
- MonthName  
- Quarter  
- Weekday fields

---

## 🧠 Key DAX Components

### Time Intelligence  
- `Total Estimated Revenue YTD`  
- `Total Estimated Revenue PY`  
- `Total Estimated Revenue YoY`  
- `Total Estimated Revenue YoY %`  

### Customer Analytics  
- `HighValue Customers Count`  
- `HighValue Customers Share`  
- `Revenue High Segment`  
- Customer segment calculation based on Lifetime Value  

### Dynamic Metrics  
- `Selected Metric Value`  
- `Selected Metric Title`  
- Metric selector table for dynamic KPI switching  

### KPI Indicators  
- `Revenue YoY Arrow` (▲ / ▼ / •)

---

## 📈 Overview Page

Includes:

- Four KPI cards  
- Line chart (Revenue vs Prior Year)  
- Year slicer  
- Region matrix with dynamic metric selection  
- Interactive metric switching via SELECTEDVALUE + SWITCH  

**Screenshot:**  
![Overview](./screenshots/overview.png)

---

## 🔍 Customer Insights Page

Contains:

- Revenue by customer segment  
- High-value customer metrics  
- High-value share (%)  
- Top 10 customers by Lifetime Value (Top N)  
- Drillthrough navigation  

**Screenshot:**  
![Customer Insights](./screenshots/customer_insights.png)

---

## 👤 Customer Detail (Drillthrough)

Displays customer-specific information:

- Customer ID  
- Region  
- Lifetime Value  
- Segment  
- Revenue contribution (optional)

**Screenshot:**  
![Customer Detail](./screenshots/drillthrough.png)

---

## 🎨 Design & Theme

This report uses a custom **Modern Minimal** theme:

- Neutral graphite (#1A1A1A, #333333)  
- Blue accent (#2962FF, #82B1FF)  
- KPI colors:  
  - green for growth (#4CAF50)  
  - red for decline (#E53935)  

Theme file:  
`theme/modern_minimal.json`

---

## 📤 Deployment

The dashboard is ready for publishing to **Power BI Service**:

1. Upload the `.pbix` file to a workspace  
2. Adjust interactions and filters  
3. Configure scheduled refresh (optional)  
4. Export as PDF or PNG for portfolio  

---

## 👨‍💻 Author

**Volodymyr Byelov**  
Data Analyst — Power BI, SQL, Python  
GitHub: *(add link here)*

---

## ⭐ Support

If you like this project, give it a ⭐ on GitHub!



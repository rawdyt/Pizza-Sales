# Pizza Sales - Dashboard

### Dashboard Link : https://app.powerbi.com/groups/me/reports/90b8b8ee-0ade-4925-8a4e-5586cf3477df/104d15949b8274d5438a?experience=power-bi

## Problem Statement

The goal of this dashboard is to analyze pizza sales performance and uncover insights related to revenue, order trends, and customer preferences.
It helps the business identify:

* Sales performance over time

* Most and least popular pizza categories

* Revenue contribution by pizza size and type

* Opportunities to increase revenue and optimize product offerings


### Steps followed 

---------------------------- Page 1 ------------------------------

- Step 1 : Load data into Power BI Desktop, dataset is a csv file.
- Step 2 : Open power query editor & in view tab under Data preview section, check "column distribution", "column quality" & "column profile" options.
- Step 3 : Also since by default, profile will be opened only for 1000 rows so you need to select "column profiling based on entire dataset".
- Step 4: Removed nulls and standardized date, time, and size formats.

-Step 5: DAX Measures Created 
 
    Avg Order_Value = [Total Revenue]/[Total Orders]

    Avg Pizza Order = [Total Pizza_sold]/[Total Orders]

    Total Orders = DISTINCTCOUNT(pizza_sales[order_id])

    Total Pizza_sold = sum(pizza_sales[quantity])

    Total Revenue = sum(pizza_sales[total_price])

-Step 6: Added filters (Slicers) for Pizza Category & Date at  
  right top corner these important filter to visualise the  
  data    
  according the needs.

- Step 5 : Added 4 KPI's using card visuals
     1) Total Revenue
     2) Avg Order_Value
     3) Total Pizza_sold
     4) Total Orders
     5) Avg Pizza Order

  Snap of the KPI's,
 ![KPI](https://raw.githubusercontent.com/rawdyt/Pizza-Sales/main/Pizza%20Sales%20KPI.jpg)

 To show the buisiest Days & Times, Best Category & Size
 We have added boxes at left side on first page

- Step 6 : Below the KPI's we have added Bar chart to show the 
  Daily trend, so that we will get to know the performance for 
  each day of the week.

- Step 7 : Are chart to show the monthly trend, o that we will  
  get to know the performance for each month.

- Step 8 : Donut chart to show the % of the sale by pizza  
  Category.

- Step 9 : Donut chart to show the % of the sale by pizza size.

- Step 10 : Funnel chart to show the sales as per the pizza   
  category.

--------- Second Page of Dashboard --------------------------

- Step 11 : The same 2 boxes at left side whcih show Best & Worst
  Seller as per the
   1) Revenue
   2) Quantity
   3) Total Orders

- Step 12 : We have added 6 Bar chart out of which 
     1) 3 shows Top 5 pizza sale by revenue, by    
        quantity, by orders.
     2) 3 show bottom 5 pizza sale by revenue, by quantity, 
        by orders.
  
  We have added buttons on the both of the sheets so that we   
  can easity move from on sheet to another.

    ![snap](https://raw.githubusercontent.com/rawdyt/Pizza-Sales/main/Screenshot%202025-11-05%20234112.jpg)

# Snapshot of Dashboard (Power BI Service)

Page 1 : 

![page 1](https://raw.githubusercontent.com/rawdyt/Pizza-Sales/main/Page%201.jpg)

Page 2 : 

![page 2](https://raw.githubusercontent.com/rawdyt/Pizza-Sales/main/Page%202.jpg)

# Insights

- Following inferences can be drawn from the dashboard;

   1)Orders are high on the Friday and Saturday.

   2)July is the month where highet orders are placed.
   
   3)Classing category pizza have generated highest sales.
   4)If we talk about size then Large pizza have generated 
  highest sales 
   

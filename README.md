# 📊 BMW Sales Dashboard (2010–2024)

This project presents an **interactive Power BI dashboard** analyzing BMW sales data from **2010 to 2024**.  
The dashboard highlights key performance metrics, trends, and insights into models, regions, fuel types, and customer preferences.

---

## 🚗 Dataset

The dataset contains **50,000 records** with the following fields:

- **Model** – BMW model (e.g., 3 Series, X1, X3, i8, 7 Series)
- **Year** – Year of sale (2010–2024)
- **Region** – Sales region (e.g., North America, Asia, Europe)
- **Color** – Car color
- **Fuel_Type** – Petrol, Diesel, Hybrid, Electric
- **Transmission** – Manual or Automatic
- **Engine_Size_L** – Engine size in liters
- **Mileage_KM** – Car mileage
- **Price_USD** – Price in USD
- **Sales_Volume** – Number of cars sold
- **Sales_Classification** – Sales category (High / Low)

---

## 📈 Dashboard Overview

### 🔹 KPIs (Top Row)
- **253M** → Total Sales Volume  
- **19T USD** → Total Revenue  
- **75.03K USD** → Average Price per Car  

### 🔹 Left Column (Trends & Technicals)
- **Line Chart – Sales Volume by Year** (2010–2024 trend)
- **Area Chart – Total Revenue by Year**
- **Scatter Plot – Engine Size vs Price** (bubble size = Sales Volume)

### 🔹 Center Column (Models & Fuel Types)
- **Bar Chart – Sales Volume by Model** (Top BMW models)
- **Stacked Bar Chart – Sales by Model & Fuel Type**

### 🔹 Right Column (Customer Preferences)
- **Donut Chart – Sales by Transmission** (Manual vs Automatic)
- **Pie Chart – Sales by Sales Classification** (High vs Low)
- **Treemap – Sales by Region** (Asia, Europe, North America, Middle East, Africa, South America)

### 🔹 Bottom Section
- **Histogram – Sales Volume by Mileage**

---

## ⚙️ DAX Calculations

### Calculated Column
```DAX
Total_Revenue = 'BMW sales data (2010-2024)'[Price_USD] * 'BMW sales data (2010-2024)'[Sales_Volume]

Total_Sales_Volume = SUM('BMW sales data (2010-2024)'[Sales_Volume])

Total_Revenue_Measure = SUM('BMW sales data (2010-2024)'[Total_Revenue])

Average_Price = AVERAGE('BMW sales data (2010-2024)'[Price_USD])

```

## 🎯 Insights From the Dashboard

Sales volume has fluctuated over the years, with peaks after 2020.

Revenue trends follow sales but highlight periods of price-driven growth.

Best-selling models include the 7 Series, i8, X1, 3 Series, and i3.

Fuel type preferences show a mix of Petrol, Diesel, Hybrid, and Electric adoption.

Transmission split is nearly 50-50 between Manual and Automatic.

Regions like Asia and Europe dominate sales volume, followed by North America.

Mileage distribution reveals customer buying behavior based on car usage.

Larger engine sizes generally correlate with higher pricing.

## 🛠 Tools Used

Power BI → Dashboard creation & visualization

DAX → Calculations & measures

Excel (XLSX) → Source dataset

## 🚀 How to Use

Download the dataset: BMW sales data (2010-2024).xlsx

Open Power BI and load the dataset

Add the calculated column and measures using the provided DAX code

Rebuild or customize the dashboard using the described layout

## 📌 Author

Mohaemn Saber
📍 Cairo, Egypt
📧 mohaemn.saber@gmail.com
📞 +201226462928

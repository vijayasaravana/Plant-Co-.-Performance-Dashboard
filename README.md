# Plant-Co-.-Performance-Dashboard

# 📊 Plant Co. Quantity Performance Dashboard (2023)

This Power BI project provides a comprehensive analysis of **Plant Co.'s** quantity performance across multiple dimensions including country, product type, and time. The report enables stakeholders to track progress, identify underperforming regions, and evaluate profitability in a visually intuitive way.

---

## 📌 Project Highlights

### 🔄 KPI Comparison
- **YTD (Year-To-Date)**, **PYTD (Prior YTD)**, and **YTD vs PYTD** performance.
- Real-time KPI cards showing key metrics:  
  - **Quantity:** 555.66K  
  - **Gross Profit:** Calculated GP% of 39.62%  
  - **PYTD Quantity:** 538.61K  
  - **Delta (YTD vs PYTD):** +17.05K  

### 📉 Visual Insights
- **Waterfall Chart:** Shows monthly quantity increase/decrease between YTD and PYTD.
- **Treemap:** Bottom 10 countries by quantity delta to identify weak regions.
- **Stacked Column Chart:** Monthly breakdown of product types (Indoor, Landscape, Outdoor).
- **Scatter Plot:** Account segmentation based on GP% and Quantity for profitability analysis.

### 🧠 Dynamic Report Titles
- Titles of charts and visuals automatically change based on user selection (e.g., Quantity, Sales, Gross Profit).
- Implemented using DAX and slicer-based SWITCH logic:

Sample:
 
  ```DAX
  _Column Chart Title = 
  SWITCH(
    TRUE(),
    SELECTEDVALUE(_Measures[Metric]) = "Quantity", "Quantity YTD & PYTD by Month",
    SELECTEDVALUE(_Measures[Metric]) = "Sales", "Sales YTD & PYTD by Month",
    SELECTEDVALUE(_Measures[Metric]) = "Gross Profit", "Gross Profit YTD & PYTD by Month",
    "Performance Overview"
  )


""


![image](https://github.com/user-attachments/assets/04153d26-4f88-48cf-9c12-02b67a81d8af)
![image](https://github.com/user-attachments/assets/10ae9b8a-2a67-4317-8c9e-a7f44506a052)
![image](https://github.com/user-attachments/assets/6e77a2f1-d604-44d8-9db8-023e2059c3ff)

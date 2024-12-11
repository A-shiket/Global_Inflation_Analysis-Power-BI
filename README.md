# **Global Inflation Analysis: Food vs. General Trends**

## **Project Overview**
This project analyzes global food and general inflation trends to assess the affordability of a healthy diet across 207 countries/regions. The data, sourced from the **FAO (Food and Agriculture Organization of the United Nations)**, is transformed and visualized in an **interactive Power BI dashboard**.

Key highlights include:
- **Calculation of Year-over-Year Inflation % for both food and general indices.**
- **Verification of calculated inflation % with FAO's incomplete inflation data to ensure accuracy.**
- **Identification of Venezuela as a significant outlier, excluded by default but made available through a slicer for detailed analysis.**

The final dashboard is designed to be intuitive, visually engaging, and user-friendly, supporting data-driven decision-making.

---

## Project Files
- **Global_Inflation_Analysis (Interactive Dashboard)**: [Explore the live interactive dashboard here](https://app.powerbi.com/view?r=eyJrIjoiZjYyYzJjMWItMjg2OC00Y2VmLWJkOTItNThhZDYzZGQ1MDY5IiwidCI6ImI4NjBiZTJmLTI1ZGMtNDc0ZC1iNzJiLTIxZmQ4YzA0NGRiMCJ9&pageName=b35b204faeea5202239e).
- **Global_Inflation_Analysis (Static Dashboard PDF)**: [Download the static PDF version here]().


---

## **Dependencies**
This project was developed using:
- **Power BI Desktop**: For data transformation, modeling, and visualization.

---

## **Dataset**
The dataset used in this project was sourced from the **FAO (Food and Agriculture Organization)** and includes:
- **Consumer Price Indices** for food and general inflation, normalized to 2015 = 100.
- **Incomplete Inflation Data: Inflation % were missing from the dataset and not included.

### **Key fields in the dataset after cleaning**:
- Country/Region
- Food Inflation %
- General Inflation %
- Inflation Gap %
- Time-based fields (Year, Month)

---

## **How I Approached the Project**

### **1. Understanding the Dataset**
- Explored the dataset to understand its structure, key fields, and overall scope.
- Calculated Year-over-Year Inflation Percentages for both food and general indices, as inflation percentages were not provided.
- Verified calculated inflation percentages against FAO’s reported (incomplete) values.


### **2. Data Preparation**
- Cleaned and transformed the raw dataset using **Power Query**:
  - Removed unnecessary columns (e.g., duplicate codes).
  - Created calculated columns like **Inflation Gap %** between General and Food index to analyze differences.
  - Sorted months using `Month Code` for accurate time-based visuals.
  - Ensured data quality by handling imputed and estimated values.
  - Excluded Venezuela, the biggest outlier, from visuals by default to avoid skewing the data. However, users can toggle its inclusion using a slicer.


### **3. Designing the Dashboard and report**
#### **Key focus areas of the dashboard**:
- **KPIs**:
  - Average Global Inflation %
  - Total Countries/Regions Included
  - Viewer controls to include/exclude Venezuela's data.
- **Visualizations**:
  - **Line Chart**: Food vs. General Inflation trends over time.
  - **Bar Charts**: Top and bottom countries by inflation rates and Inflation gap % for all countries/regions.
  - **Scatter Plot**: Correlation between Food and General Inflation across countries.
  - **Map Visual**: Average inflation rates across the globe (enabled via Bing Maps).
- **Interactivity**:
  - Slicers:
    -Country/Region, Year, Quarter, and Outlier Classification:
            -"Regular" excludes Venezuela by default.
            -"Include Outlier" allows users to visualize the skew caused by Venezuela's data.
  - Custom tooltips for deeper insights into inflation gaps.

---

## **Insights and Takeaways**
### **Key findings from the analysis**:
1. **Food Inflation Consistently Higher**:
   - Across all regions and time periods, **food inflation consistently exceeds general inflation**, reflecting the rising cost of food globally.
   
2. **Largest Inflation Gaps**:
   - Countries like **Lebanon** and **Zimbabwe** exhibit high negative gaps, meaning food inflation is significantly higher than general inflation.
   
3. **Venezuela as a Major Outlier**:
   - With inflation rates exceeding thousands of percent, **Venezuela dramatically skews the data**. By default, its data is excluded from visuals for clearer insights, but viewers can toggle its inclusion using a slicer.

4. **Top and Bottom Performers**:
   - **South Sudan** and **Sudan** lead in overall inflation rates, while countries like **Switzerland** and **Japan** maintain the lowest levels of inflation.

---

## **Acknowledgments**
- **Data Source**: [FAO (Food and Agriculture Organization of the United Nations)]([https://www.fao.org](https://www.fao.org/faostat/en/#data/CAHD))
- This project was designed using **Power BI Desktop** to showcase global inflation trends and their impact on food affordability.

---

## **How to View the Dashboard**
1. **Power BI Service**:
   - View the interactive dashboard online: []
2. **PDF Export**:
   - Access the static version of the dashboard through the Global_Inflation_Analysis.pdf file.

---

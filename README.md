# Myntra Product & Marketplace Analysis  
**Excel + Power BI Capstone Project**

## 📌 Project Overview

This project is an end-to-end **data analytics capstone** built using a real-world, scraped Myntra product catalog dataset.
The focus of this project is **catalog and marketplace analysis**, rather than sales or revenue forecasting.

## 🎯 Business Questions Addressed

This analysis was designed to answer practical business questions such as:

- How is Myntra’s product catalog distributed across price ranges?
- Which brands dominate the catalog by volume?
- Do heavy discounts actually improve customer ratings?
- How do pricing and discounts vary across brands and product attributes?
- Does a higher price consistently lead to better customer perception?

## Dataset Summary

- **Source:**: [**Order Details**](https://github.com/radhasiingh/Power-BI-Project-1/blob/main/Details.csv)
- **Size:** ~52,120 raw product records
- **Nature:** Publicly available product metadata

> ⚠️ *Disclaimer:*  
> This dataset is used strictly for learning and portfolio purposes.  
> It does **not** represent actual Myntra sales data or internal business metrics.

## Data Cleaning & Preparation (Excel)

Excel was used as the first stage of the analytics workflow, closely mirroring real industry practices.

### Key Steps Performed
- Removed duplicate and invalid product records  
- Converted price, MRP, ratings, and review counts to numeric formats  
- Recalculated discount percentage using a consistent formula  
- Standardised brand names using text functions  
- Extracted product attributes (fit, fabric, wash type) from descriptions  
- Handled missing and inconsistent values  
- Created analytical buckets for:
  - Price ranges  
  - Rating categories 

## 📊 Power BI Dashboard

The cleaned dataset was loaded into Power BI to build an interactive, business-ready dashboard.

### Dashboard Pages

#### 1️⃣ Marketplace Overview
- Total products & brands
- Average price and discount
- Weighted average rating
- Product distribution by price and rating buckets

![Marketplace Overview](visuals/dashboard_overview.png)

#### 2️⃣ Brand-Level Catalog & Positioning
- Top brands by catalog size
- Top brands by average discount
- Brand positioning using:
  - Average price
  - Weighted average rating
  - Product count

 ![Brand Analysis](visuals/brand_analysis.png)

#### 3️⃣ Pricing & Discount Behavior
- Discount intensity across price segments
- Rating comparison across discount levels
- Identification of discount-heavy catalog segments

![Pricing & Discount](visuals/pricing_discount.png)

#### 4️⃣ Fit-Based Product Performance
- Product distribution by fit type
- Average price and discount by fit
- Price vs rating relationship across fits

![Fit Analysis](visuals/fit_analysis.png)

## 🧠 Key Insights

- A small number of brands contribute a disproportionately large share of the catalog
- Heavy discounting does **not** consistently lead to better customer ratings
- Mid-priced products often achieve competitive ratings without extreme discounts
- Higher prices do not always guarantee higher perceived quality

## ⚠️ Assumptions & Limitations

- No sales or revenue data available
- Ratings are treated as post-purchase customer sentiment
- Discounts analyzed are listed discounts, not realized transaction discounts
- Product attributes are extracted from free-text descriptions and may not be fully accurate

## Tools & Skills Demonstrated

- **Excel:** Data cleaning, text functions, logical functions, PivotTables, EDA  
- **Power BI:** Data modeling, DAX measures, dashboard design  
- **Analytical Skills:** Business reasoning, KPI design, insight communication  

*This repository is part of my analytics portfolio and is intended for learning and demonstration purposes.*

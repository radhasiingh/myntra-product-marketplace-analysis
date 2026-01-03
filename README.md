## Myntra Product & Marketplace Analysis (Excel + Power BI)

### 📌 Project Overview
This project analyzes a fashion marketplace product catalog to understand pricing structure, discounting behavior, brand presence, and customer rating patterns at a product (SKU) level.
The objective is to work with a large, messy, real-world dataset and convert it into clean, marketplace insights using Excel for data preparation and Power BI for analysis and visualization.
This is a descriptive catalog analysis, not a sales, revenue, or predictive study.

### Dataset Summary
- Source: Public Kaggle dataset of Myntra product listings
  Link: [Myntra Sales Dataset](https://www.kaggle.com/datasets/skmewati/myntra-sales-dataset)
- Raw dataset: 52,120 product records across 417 brands
- Final Cleaned dataset: 16,928 usable product SKUs across 369 brands
- Granularity: Each row represents a single listed product SKU
- Core fields: Brand, price, MRP, discount %, rating, number of ratings, product description

### Business Problems Addressed
The analysis is designed to answer practical marketplace questions such as:
1. How is the product catalog distributed across different price ranges?
2. How are products spread across customer rating categories?
3. Which brands dominate the catalog by product count?
4. How do discount levels vary across price segments and brands?
5. How do pricing, discounting, and ratings differ across product fit types?

### Data Preparation & Assumptions (Excel)
To ensure interpretable and defensible analysis, the following steps and decisions were taken:
1. Raw data was preserved separately; all transformations were performed on a cleaned working sheet.
2. Duplicate and invalid records were removed based on full-row validation.
3. Price, MRP, discount, rating, and rating count fields were converted from text to numeric formats.
4. Discount percentage was recalculated using a consistent formula across all products.
5. Brand names were standardized to enable accurate brand-level aggregation.
6. Analytical buckets were created for:
- Price ranges
- Rating categories
7. Product fit types were derived from free-text product descriptions using rule-based keyword matching.
8. Each row was treated as an independent SKU; no aggregation at style or product-family level was attempted.

### Analysis & Insights
1. The product catalog is primarily concentrated in mid-price ranges, with fewer products at extreme low and high price points.
2. Customer ratings are largely clustered in the Average to Good categories, showing limited spread across most of the catalog.
3. A small number of brands contribute a disproportionately large share of total product listings, while most brands operate at smaller catalog sizes.
4. Discounting is widespread across the marketplace, with a significant portion of products offered at high discount levels, particularly in lower and mid-price segments.
5. Products with very high discounts do not consistently receive higher customer ratings, indicating discounting alone is not a strong signal of perceived quality.
6. Higher-priced products do not reliably achieve higher ratings, suggesting that price premium does not guarantee better customer sentiment.
7. Slim and Regular fits dominate the catalog, while some fit types are positioned at relatively higher average prices.
8. Even premium-priced fits continue to rely on discounting, highlighting the importance of discounts across the fashion catalog.

### Scope & Limitations
- The dataset contains no sales, revenue, quantity, or customer-level information.
- Discounts analyzed are listed discounts derived from price and MRP, not realized transaction discounts.
- Customer ratings and rating counts are used as provided, without bias correction or behavioral modeling.
- Product fit types are derived from free-text descriptions using rule-based keyword matching and may contain classification noise.
- The dataset represents a static snapshot of the catalog, with no time-based or trend analysis possible.

### Tools Used
- Microsoft Excel: Data cleaning, transformation, EDA, pivot-based analysis, power query
- Power BI: Data modeling, DAX measures, interactive dashboards

### Dashboards
#### 1️⃣ Marketplace Overview
##### Purpose: Provide a high-level snapshot of the marketplace.
![Marketplace Overview](overview.png)

#### 2️⃣ Brand-Level Catalog & Positioning
##### Purpose: Understand how brands compete within the marketplace.
![Brand-Level Analysis](brands.png)

#### 3️⃣ Pricing & Discount Behavior
##### Purpose: Examine how discounting relates to pricing and customer ratings.
![Pricing & Discount Analysis](pricing_and_discount.png)

#### 4️⃣ Fit-Based Product Performance
##### Purpose: Analyse product performance across different fit types.
![Fit-Based Analysis](fit.png)

> **Disclaimer**  
> A publicly available dataset is used for the project and doesn't represent Myntra's internal business data.
> This project is for learning and portfolio demonstration purposes only.

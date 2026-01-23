# Zameen.com Real Estate Analysis: Price Drivers in Pakistan

## 📄 Executive Summary
This project presents an exploratory data analysis (EDA) of real estate listings scraped from Zameen.com. The objective is to identify the key factors driving property prices in Pakistan. Through structured statistical analysis and visual exploration, the study evaluates the influence of location, property size, room counts, and property purpose on pricing trends.

The analysis reveals that **location** and **covered area** are the strongest determinants of price. Significant price variation exists across cities, indicating a strong spatial dependence in Pakistan’s real estate market.

---

## ❓ Business Question
> **"What are the primary drivers of property prices in Pakistan?"**

This report aims to uncover patterns, trends, and relationships among key variables to provide actionable insights for buyers, sellers, and investors.

---

## 🛠️ Methodology

### Data Source
* **Origin:** Scraped from Zameen.com, Pakistan’s largest real estate marketplace.
* **Format:** Structured CSV/Excel data.

### Data Preparation & Cleaning
1. **Cleaning:** Removed duplicate rows/columns and handled blank entries.
2. **Smart Imputation:** Missing "Area" values were handled by grouping properties with similar specifications (Location + No. of Bedrooms) and calculating the group average.
3. **Type Conversion:** Standardized numerical and categorical data types for consistency.
4. **Feature Engineering (Luxury Score):** To handle sparse variables like swimming pools, generators, and security guards, I introduced a **Luxury Score**. This metric aggregates these features into a single value to measure their collective impact on property price.

### Analytical Approach
* **Descriptive Statistics:** Used to understand distributions and central tendencies.
* **Visualizations:** Employed histograms, boxplots, and scatter plots to identify trends and outliers.
* **Comparative Analysis:** Conducted across cities and property types (Sale vs. Rent).

---

## 📈 Key Findings

* **Location as a Primary Driver:** Major urban centers exhibit substantially higher average prices, confirming that location is the most influential factor.
* **Impact of Size:** There is a strong positive relationship between covered area and price, though the price-per-unit area fluctuates by locality.
* **Diminishing Returns on Rooms:** While more bedrooms/bathrooms generally increase price, the incremental value diminishes beyond a certain count.
* **Market Outliers:** High-end luxury properties create a right-skewed distribution, primarily concentrated in premium sectors.

---

## 💡 Recommendations

### For Buyers & Investors
* **Focus on growth:** Target emerging localities where price-per-unit area is lower but urban development is rising.
* **Valuation:** Use price-per-area metrics rather than absolute prices for more accurate investment comparisons.

### For Sellers & Platforms
* **Highlight Features:** Emphasize locational advantages and total covered area, as these drive the highest value.
* **Analytics:** Real estate platforms should implement automated price estimation models using location and size as primary predictors.

---

## 💻 Tech Stack
* **Language:** Python
* **Libraries:** Pandas, Matplotlib, Seaborn, NumPy
* **Tools:** Jupyter Notebook

---

## 📂 Project Structure
```text
├── data/               # Raw and cleaned datasets
├── notebooks/          # Jupyter notebooks with EDA and visualizations
├── visualizations/     # Exported images and charts
└── README.md           # Project documentation

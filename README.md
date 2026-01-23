# Zameen.com Real Estate Analysis: Price Drivers in Pakistan
📋 Project Overview
This project performs an Exploratory Data Analysis (EDA) on real estate listings scraped from Zameen.com. The primary objective is to identify and quantify the key factors that drive property prices across Pakistan's diverse real estate market.

❓ Business Question
"What are the primary determinants of property prices in Pakistan, and how do they vary across different urban landscapes?"

🚀 Key Features
Data Cleaning Pipeline: Systematic removal of duplicates and handling of structural inconsistencies.

Advanced Imputation: Used a group-based mean strategy (Location + Bedrooms) to accurately fill missing values in property area.

Feature Engineering: Developed a "Luxury Score" to quantify the impact of niche amenities (e.g., swimming pools, security guards, generators) into a single metric.

Spatial Analysis: Comparative study of price trends across major Pakistani cities and localities.

🛠️ Methodology
1. Data Preparation
Cleaning: Removed redundant rows/columns and corrected data types for numerical consistency.

Imputation: Missing area values were filled by grouping similar listings based on Location and No. of Bedrooms, then applying the average area of that specific group.

Feature Engineering: Instead of treating rare amenities (swimming pools, generators) as individual variables, I introduced a Luxury Score. This counts the presence of high-end features to measure their collective impact on valuation.

2. Analytical Approach
Descriptive Statistics: To understand central tendencies and price distributions.

Visual Exploration: Used Histograms, Boxplots, and Scatter plots to identify trends, correlations, and outliers.

Comparative Analysis: Segmented data by city and property purpose (Sale vs. Rent).

📈 Key Findings
Location is King: Location remains the strongest predictor of price, with significant variance even within the same city.

Diminishing Returns: While bedrooms and bathrooms increase value, the marginal price increase drops significantly after a certain threshold.

Size vs. Value: Covered area has a strong positive correlation with price, but the price-per-unit area is heavily dependent on the locality's prestige.

Market Skew: The market is heavily right-skewed due to high-end luxury outliers in premium sectors.

💡 Recommendations
For Investors: Target emerging localities with lower price-per-unit area but high urban growth potential.

For Sellers: Focus marketing efforts on "Covered Area" and "Locational Advantages," as these are the primary value drivers.

For Platforms: Implement automated valuation models (AVMs) using location and size as core features.

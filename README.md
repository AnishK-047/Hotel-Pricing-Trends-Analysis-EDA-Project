🏨 Hotel Pricing Trends – Exploratory Data Analysis (Booking.com)


📌 Project Overview

This project analyzes hotel pricing trends using data scraped from Booking.com. It focuses on how location, star ratings, review scores, room types, and booking features influence hotel prices. The analysis helps identify pricing patterns useful for travelers, hotels, and travel platforms.



🔧 Tools & Technologies

Python

Requests, BeautifulSoup (Web Scraping)

Pandas (Data Cleaning & Manipulation)

Matplotlib, Seaborn (Data Visualization)



📂 Dataset Summary

Total Rows: 62,361 (Raw) → 434 (Cleaned)

Columns: 8

Key Fields: Hotel Name, Location, Price, Star Rating, Review Score, Room Type, Booking Features

Wide variation in pricing with several high-value outliers

Minimal missing values after cleaning



🧹 Data Cleaning & Preparation

Removed duplicate records

Cleaned noisy hotel names and room descriptions

Converted price to numeric format

Filled missing star ratings and review scores

Extracted clean location fields

Categorized review scores and created price bins



📊 Exploratory Data Analysis
Univariate Insights

Most hotel prices fall below ₹5000, with a right-skewed distribution

Review categories are dominated by “Very Good” and “Good”

3-star and 4-star hotels are the most common

Bivariate Insights

High review scores do not guarantee higher prices

Strong positive relationship between Star Rating and Price

5-star hotels show the widest and highest price range

Multivariate Insights

Location has a major impact on pricing

Cities like Bānskhoh and Bodh Gaya have higher average prices

Budget clusters found in New Delhi, Vijayawada, Calicut

Correlation summary:

Price ↗ with Star Ratings (moderate correlation)

Price vs Review Score = weak correlation



🔎 Key Findings

Star Ratings and Location are the strongest drivers of hotel pricing

Review Scores act as a baseline expectation rather than a price driver

Some locations show premium pricing while others remain budget-friendly

Many affordable hotels still maintain high review scores



🚧 Challenges Faced

CAPTCHA and anti-scraping restrictions

Inconsistent HTML structure across listings

Noisy hotel names and unstructured data

Processing a large dataset efficiently

🏁 Conclusion

Hotel pricing is influenced more by location and star ratings than by customer reviews. This EDA provides a clear understanding of pricing behavior across different destinations and hotel categories, offering value for both customers and businesses.

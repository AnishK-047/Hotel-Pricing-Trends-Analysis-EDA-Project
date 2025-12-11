# 🏨 Hotel Pricing Trends – Exploratory Data Analysis (Booking.com)

## 📌 Project Overview
This project analyzes hotel pricing trends using data scraped from Booking.com. It focuses on how **location**, **star ratings**, **review scores**, **room types**, and **booking features** influence hotel prices. The analysis helps identify pricing patterns for both travelers and hotel businesses.

---

## 🔧 Tools & Technologies
- Python  
- Requests, BeautifulSoup (Web Scraping)  
- Pandas (Data Cleaning & Manipulation)  
- Matplotlib, Seaborn (Visualizations)  
- Jupyter Notebook  

---

## 📂 Dataset Summary
- **62,361 rows (Raw)** → **434 rows (Cleaned)**  
- Total Columns: 8  
- Key Fields:  
  - Hotel Name  
  - Location  
  - Price  
  - Star Rating  
  - Review Score  
  - Review Text  
  - Room Type  
  - Booking Features  
- Large variation in price; several high-value outliers  
- Minimal missing values after cleaning  

---

## 🧹 Data Cleaning & Preparation
- Removed duplicates  
- Cleaned noisy hotel names and unstructured text  
- Converted price to numeric format  
- Filled missing review scores and star ratings  
- Extracted clean location fields  
- Created price bins and review score categories  

---

## 📊 Exploratory Data Analysis

### 🔹 Univariate Insights
- Most hotel prices fall below **₹5000**, with a right-skewed distribution  
- Review categories dominated by **“Very Good”** and **“Good”**  
- 3-star and 4-star hotels are the most common  

### 🔹 Bivariate Insights
- Higher review scores do **not** mean higher prices  
- **Star Rating** has a strong positive relationship with price  
- 5-star hotels show the highest and widest price range  

### 🔹 Multivariate Insights
- **Location is a major driver of hotel pricing**  
- Cities like *Bānskhoh* and *Bodh Gaya* have higher average prices  
- Budget-friendly clusters: *New Delhi*, *Vijayawada*, *Calicut*  
- Correlation Summary:  
  - Price ↗ with Star Ratings (moderate)  
  - Price vs Review Score = weak  

---

## 🔎 Key Findings
- **Star Ratings** and **Location** influence hotel pricing far more than reviews  
- **Review Scores** act as a baseline expectation, not a pricing factor  
- Many low-cost hotels still maintain high customer satisfaction  

---

## 🚧 Challenges Faced
- CAPTCHA & anti-scraping restrictions while collecting data  
- Inconsistent HTML structure  
- Noisy hotel names and messy attributes  
- Processing 62k+ rows efficiently  

---

## 🏁 Conclusion
Hotel pricing is primarily driven by **Star Ratings** and **Location**, while customer reviews show minimal price influence. This analysis delivers useful insights for travelers, hotel owners, and online booking platforms.

---

## 📁 Project Structure
```
Hotel_Pricing_EDA/
│
├── data/
│   ├── raw_data.csv
│   ├── cleaned_data.csv
│
├── notebooks/
│   ├── 01_web_scraping.ipynb
│   ├── 02_data_cleaning.ipynb
│   ├── 03_eda_visualizations.ipynb
│
├── src/
│   ├── scraping.py
│   ├── cleaning.py
│   ├── analysis.py
│
├── visuals/
│   ├── price_distribution.png
│   ├── star_rating_vs_price.png
│   ├── heatmap.png
│
├── README.md
├── requirements.txt
└── .gitignore
```

---


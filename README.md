## Bestseller Prediction Analysis (Python)

## Executive Summary

This project analyzes data from the Top 100 Amazon Bestseller lists using Excel, Python, and Power BI to identify key patterns in book performance over recent years. The objective is to support data-driven decision-making for book retailers by informing stocking strategies for 2026–2027.The analysis addresses the following questions:

1. Which titles and authors should receive the majority of shelf space and inventory allocation?
2. Which books demonstrate consistent demand and represent low-risk investments?
3. Which authors should be prioritized, monitored, and further promoted based on performance?

Additionally, the analysis supports inventory planning by identifying titles with the highest likelihood of sustained demand, helping retailers minimize stock shortages and optimize sales in the upcoming market cycle.
---

##Business Problem

Major book retailers worldwide face ongoing inventory allocation challenges due to limited shelf space, a large volume of titles, and continuous new releases. These constraints create several key challenges:

1. Demand Uncertainty: Retailers must determine which books will sustain popularity and which will decline, making it difficult to balance inventory effectively.
2. Financial Risk: Poor stocking decisions can lead to unsold inventory or missed sales opportunities, directly impacting revenue.
3. Author and Series Strategy: Retailers must decide which authors and series to prioritize, promote, and expand in-store based on their ability to drive consistent demand.
   
In essence, the core challenge is deciding which books to stock, in what quantity, and how to allocate shelf space under conditions of uncertainty.

This recent years trands explorations will allow to answer some of those question by proving key insights based on real world data anad consumer's behaviour. Aamazon's besteller's list comaopred to other lists such as the new New York Times, even if less data is colected and the future is unpredictabel, provides the major vantage that reflects actual recent trands, preferences and on what readers and non reader alike are willing to spend their money on.

Business Analysis:
> **Which books are most likely to remain bestsellers, and what should retailers stock in 2026?**

Already from the first analysis, comparing metrics such as numbers of rwviews, rating, apparences and giving a populairty score, the top names are already quite clear. "Fourth Wing" by Rebecca Yarrow as well as "The Housemade" dominate the ranking by far followed by "Verity", "Onix Storm" and "Iron Flame.

![image](https://github.com/user-attachments/assets/eeabe6dd-406f-4dd6-a595-3e7887c80c04)





---

## 📊 Dataset
- Source: [Add source if available]
- Timeframe: 2024–2025 (2023 excluded due to inconsistencies)
- Key Features:
  - Title
  - Author
  - Price
  - Rating
  - Number of Reviews
  - Year

---

## 🧹 Data Cleaning & Preparation
- Handled missing values (e.g., Author, Price)
- Converted price to numeric format
- Standardized book titles (removed duplicates and variations)
- Created a **Clean Title** field to merge editions
- Excluded 2023 due to inconsistent and skewed data

---

## 🧠 Methodology
- Aggregated data by book title
- Created key metrics:
  - Average Rating
  - Average Number of Reviews
  - Appearances (frequency across dataset)
- Built a **Popularity Score** combining:
  - Demand (reviews)
  - Quality (rating)
  - Consistency (appearances)
- Identified top-performing books based on this score

---

## 📈 Key Insights

- **Top Performers**: Certain books (e.g., *Fourth Wing*, *The Housemaid*) consistently dominate across years.
- **Stable Demand**: Minimal variation in performance suggests sustained popularity.
- **Series & Author Strength**: Multiple titles from the same authors/series perform strongly.
- **Market Concentration**: A small number of books drive the majority of engagement.

---

## 💡 Business Recommendations

- Prioritize stocking top-performing titles with consistent demand  
- Invest in books from high-performing authors and series  
- Maintain inventory of multiple editions for popular titles  
- Monitor similar future releases from proven authors  

---

## 📊 Visualizations

*(Insert your charts here)*

Example:
```markdown
![Top Books](images/top_books.png)

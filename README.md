## Bestseller Prediction Analysis (Python)

## Executive Summary

This project analyzes data from the Top 100 Amazon Bestseller lists using Excel, Python, and Power BI to identify key patterns in book performance over recent years. The objective is to support data-driven decision-making for book retailers by informing stocking strategies for 2026–2027.The analysis addresses the following questions:

1. Which titles and authors should receive the majority of shelf space and inventory allocation?
2. Which books demonstrate consistent demand and represent low-risk investments?
3. Which authors should be prioritized, monitored, and further promoted based on performance?
--
Additionally, the analysis supports inventory planning by identifying titles with the highest likelihood of sustained demand, helping retailers minimize stock shortages and optimize sales in the upcoming market cycle.
---

## Business Problem

Major book retailers worldwide face ongoing inventory allocation challenges due to limited shelf space, a large volume of titles, and continuous new releases. These constraints create several key challenges:

1. Demand Uncertainty: Retailers must determine which books will sustain popularity and which will decline, making it difficult to balance inventory effectively.
2. Financial Risk: Poor stocking decisions can lead to unsold inventory or missed sales opportunities, directly impacting revenue.
3. Author and Series Strategy: Retailers must decide which authors and series to prioritize, promote, and expand in-store based on their ability to drive consistent demand.
   
In essence, the core challenge is deciding which books to stock, in what quantity, and how to allocate shelf space under conditions of uncertainty.

This recent years trands explorations will allow to answer some of those question by proving key insights based on real world data anad consumer's behaviour. Aamazon's besteller's list comaopred to other lists such as the new New York Times, even if less data is colected and the future is unpredictabel, provides the major vantage that reflects actual recent trands, preferences and on what readers and non reader alike are willing to spend their money on.

Business Analysis:

> **Which books sold the most copyes in recent years and are in constant high demnand?**

We will tackle first the upper part of our ranking.

Already from the first analysis, comparing metrics such as numbers of rwviews, rating, apparences and giving a populairty score, the top names are quite clear.
"Fourth Wing" by Rebecca Yarrow and "The Housemade" by Feida MccFedden dominate the ranking, closley followed by "Verity", "Onix Storm" and "Iron Flame.


![image](https://github.com/user-attachments/assets/eeabe6dd-406f-4dd6-a595-3e7887c80c04)


However, the most interesting insight, that will also prove to be a pattern during this first glance at our data is that: It is not the title per-se that seems to drive sales and demand, but the series.

This is crucilal because we can drawn a precious consumer's behavior insight that can be epxploited in favour of retailer. It is in fact clear that the reader that buys the first book of the series is very likely to also follow through with the next book of the serie, and then again and again, in doing so creating a chain reaction of repeat-purchase.

Those titles are clearly nothing less than potential goldmine for retailers, and they shoudl have priority in stocking and shelving.

As for the second part of our ranking confirms the repeat buy phenomenon.

![IMG_3345](https://github.com/user-attachments/assets/0097d7b8-6e42-4433-ad07-fb404aad5f26)

"The Housemaid is Watching".
"The Housemaid's Secret"
"A Court Of Thorns and Roses".
"A Court Of Myst And Fury".
"A Court of Wings and Ruins".





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

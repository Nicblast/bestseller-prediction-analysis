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

## Business Analysis

Which books have sold the most copies in recent years and demonstrate sustained high demand?

We begin by analyzing the highest-performing titles based on a combination of metrics, including number of reviews, ratings, frequency of appearance, and an aggregated popularity score across the years 2023, 2024 and 2025 for the bigger picture. And then we narrowed down our dataset to 2024 and 2025 find out the very recent trrands and patterns of the readers.

From our "popularity score" analysis, clear leaders emerge. “Fourth Wing” by Rebecca Yarros and “The Housemaid” by Freida McFadden consistently dominate the rankings, closely followed by titles such as “Verity”, “Onyx Storm”, and “Iron Flame”.

This is confirmed in our chart:

![IMG_3345](https://github.com/user-attachments/assets/485e79d5-f239-4616-a081-2f3666dc501a)

A key insight from this initial view is that demand appears to be driven less by individual standalone titles and more by book series. This pattern is crucial from a retail perspective, as it suggests strong cross-title engagement within the same author universe.

In practice, readers who purchase the first book in a series are highly likely to continue with subsequent installments, creating a repeat purchase effect. This behavior significantly increases the long-term value of series-based titles.
As a result, these books represent high-value inventory for retailers and should be prioritized in both stocking decisions and shelf placement.

This pattern is further reinforced in the lower portion of the ranking, where multiple entries from the same series continue to appear among top-performing titles:

![IMG_3345](https://github.com/user-attachments/assets/a73d2e24-bbc9-47bb-9ed6-8fd341beec5f)

Examples include:
“The Housemaid’s Secret”, “The Housemaid Is Watching”
“A Court of Thorns and Roses”, “A Court of Mist and Fury”, “A Court of Wings and Ruin”
These observations confirm the repeat-purchase phenomenon and highlight the importance of series-driven demand in driving sustained bestseller performance

## Dual Track Market Value

Which titles bring the lowest risk and guarantee the highest ROI?

Before narrowing down our data, "Normalization" was used to scale review data and enable fair comparison (comparison only) across titles and years by reducing the impact of extreme values. This helped identify relative performance and consistency patterns, although data inconsistencies in 2023 limited its reliability for final analysis.

![IMG_3367](https://github.com/user-attachments/assets/a66aff77-75c0-4b7c-a395-2c869edbcfa0)

Interestingly, the normalized data identifies "The Housemaid" as the absolute market benchmark, maintaining a maximum saturation score of 1.0 that serves as the ceiling for all the other titles.

![IMG_3366](https://github.com/user-attachments/assets/f4399a33-7314-4a98-9562-559001cf2c19)

While Fourth Wing and its sequels show strong, stable engagement, older hits like the ACOTAR series have seen their relative impact drop significantly, signaling a transition from active growth to legacy status. 

Consequently, this seemingly contrasting information from the previous chart might suggest that the 2026/27 strategy should focus on the rising momentum of specific sequels like The Housemaid's Secret, which are successfully converting existing brand loyalty into sustained market dominance.

The insights integrate perfectly because they map the two different ways a book dominates a market: viral momentum versus absolute volume. While the first chart shows Fourth Wing as the fastest-growing breakout star in terms of raw popularity, the normalized heatmap reveals that The Housemaid remains the industry’s "gold standard" for consistent, peak-level engagement. 

Together, these datasets suggest a dual-track strategy for 2026/27 that prioritizes maintaining the reliable floor established by The Housemaid while at the same time aggressively scaling the high-velocity growth seen in the Fourth Wing and Onyx Storm series.

## The Popularity Score applied to authors

What authors should be given priority in the following years with new releases?

![IMG_3369](https://github.com/user-attachments/assets/0378176c-044e-4d54-a67b-e923a3306b2a)

To finish off our analysis, we also applied our popularity score to authors. It did not come as a surprise that although the dataset was now limited to 2024–2025, it further confirmed the dual-track market value insight we obtained from the full three-year comparison. This confirms that, despite the 2024 performance plateau, established authors like Freida McFadden continue to provide a high-performance ceiling and a guaranteed revenue floor that anchors the market. 

Consequently, priority for 2026/27 releases should be reserved for McFadden to maintain this absolute stability, while simultaneously fast-tracking new titles from Rebecca Yarros to capitalize on the explosive, viral momentum that currently drives the industry's growth curve.

Ultimately, these authors represent the "critical path" for retail success, as their upcoming releases are what the vast majority of readers entering a bookstore or browsing Amazon are most likely to pre-order or buy on sight.

--


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

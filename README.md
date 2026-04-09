## Bestseller Prediction Analysis (Python)

## Executive Summary

This project analyzes data from the Top 100 Amazon Bestseller lists using Excel, Python, and Power BI to identify key patterns in book performance over recent years. The objective is to support data driven decision-making for book retailers by informing stocking strategies for 2026–2027. The analysis addresses the following questions:

1. Which titles and authors should receive the majority of shelf space and inventory allocation?
2. Which books demonstrate consistent demand and represent low-risk investments?
3. Which authors should be prioritized, monitored, and further promoted based on performance?
--
Additionally, the analysis supports inventory planning by identifying titles with the highest likelihood of sustained demand, helping retailers minimize stock shortages and optimize sales in the upcoming market cycle.
---

## Business Problem:

Major book retailers worldwide face ongoing inventory allocation challenges due to limited shelf space, a large volume of titles, and continuous new releases. These constraints create several key challenges:

**1. Demand Uncertainty:** Retailers must determine which books will sustain popularity and which will decline, making it difficult to balance inventory effectively.
**2. Financial Risk:** Poor stocking decisions can lead to unsold inventory or missed sales opportunities, directly impacting revenue.
**3. Author and Series Strategy:** Retailers must decide which authors and series to prioritize, promote, and expand in-store based on their ability to drive consistent demand.
   
In essence, the core challenge is deciding which books to stock, in what quantity, and how to allocate shelf space under conditions of uncertainty.

This recent years trands explorations will allow to answer some of those question by proving key insights based on real world data anad consumer's behaviour. Aamazon's besteller's list comaopred to other lists such as the new New York Times, even if less data is colected and the future is unpredictabel, provides the major vantage that reflects actual recent trands, preferences and on what readers and non reader alike are willing to spend their money on.

## Analysis:

**Which books have sold the most copies in recent years and demonstrate sustained high demand?**

We begin by analyzing the highest-performing titles based on a combination of metrics, including number of reviews, ratings, frequency of appearance, and an aggregated popularity score across the years 2023, 2024 and 2025 for the bigger picture. And then we narrowed down our dataset to 2024 and 2025 find out the very recent trrands and patterns of the readers.

From our "popularity score" analysis, clear leaders emerge. “Fourth Wing” by Rebecca Yarros and “The Housemaid” by Freida McFadden consistently dominate the rankings, closely followed by titles such as “Verity”, “Onyx Storm”, and “Iron Flame”.

This is confirmed in our chart:

![IMG_3345](https://github.com/user-attachments/assets/485e79d5-f239-4616-a081-2f3666dc501a)

A key insight from this initial view is that demand appears to be driven less by individual standalone titles and more by book series. This pattern is crucial from a retail perspective, as it suggests strong cross-title engagement within the same author universe.

In practice, readers who purchase the first book in a series are highly likely to continue with subsequent installments, creating a repeat purchase effect. This behavior significantly increases the long-term value of series-based titles.
As a result, these books represent high-value inventory for retailers and should be prioritized in both stocking decisions and shelf placement.

This pattern is further reinforced in the lower portion of the ranking, where multiple entries from the same series continue to appear among top-performing titles:


![IMG_3345](https://github.com/user-attachments/assets/a73d2e24-bbc9-47bb-9ed6-8fd341beec5f)


**Examples include:**
“The Housemaid’s Secret”, “The Housemaid Is Watching”
“A Court of Thorns and Roses”, “A Court of Mist and Fury”, “A Court of Wings and Ruin”
These observations confirm the repeat-purchase phenomenon and highlight the importance of series-driven demand in driving sustained bestseller performance

## Dual Track Market Value:

**Which titles bring the lowest risk and guarantee the highest ROI?**

Before narrowing down our data, "Normalization" was used to scale review data and enable fair comparison (comparison only) across titles and years by reducing the impact of extreme values. This helped identify relative performance and consistency patterns, although data inconsistencies in 2023 limited its reliability for final analysis.



![IMG_3367](https://github.com/user-attachments/assets/a66aff77-75c0-4b7c-a395-2c869edbcfa0)



Interestingly, the normalized data identifies "The Housemaid" as the absolute market benchmark, maintaining a maximum saturation score of 1.0 that serves as the ceiling for all the other titles.


![IMG_3366](https://github.com/user-attachments/assets/f4399a33-7314-4a98-9562-559001cf2c19)


While Fourth Wing and its sequels show **strong, stable engagement,**  older hits like the *+ACOTAR** series have seen their relative impact drop significantly, signaling a transition from active growth to legacy status. 

Consequently, this seemingly contrasting information from the previous chart might suggest that the 2026/27 strategy should focus on the rising momentum of specific sequels like The Housemaid's Secret, which are successfully converting existing brand loyalty into sustained market dominance.

The insights integrate perfectly because they map the two different ways a book dominates a market: viral momentum versus absolute volume. While the first chart shows Fourth Wing as the fastest-growing breakout star in terms of raw popularity, the normalized heatmap reveals that The Housemaid remains the industry’s "gold standard" for consistent, peak-level engagement. 

Together, these datasets suggest a dual-track strategy for 2026/27 that prioritizes maintaining the reliable floor established by The Housemaid while at the same time aggressively scaling the high-velocity growth seen in the Fourth Wing and Onyx Storm series.

## The "Popularity Score" applied to authors:

**Which author should be given priority in the following years with new releases?** 

![IMG_3369](https://github.com/user-attachments/assets/0378176c-044e-4d54-a67b-e923a3306b2a)

To finish off our analysis, we also applied our **popularity score** to authors. It did not come as a surprise that although the dataset was now limited to 2024–2025, it further confirmed the dual-track market value insight we obtained from the full three year comparison. This confirms that, despite the 2024 performance plateau, established authors like Freida McFadden continue to provide a high performance ceiling and a guaranteed revenue floor that anchors the market. 

Consequently, priority for 2026/27 releases should be reserved for McFadden to maintain this absolute stability, while simultaneously fast-tracking new titles from Rebecca Yarros to capitalize on the explosive, viral momentum that currently drives the industry's growth curve.

Ultimately, these authors represent the "critical path" for retail success, as their upcoming releases are what the vast majority of readers entering a bookstore or browsing Amazon are most likely to pre-order or buy on sight.

--

## Dataset:

* **Source:** Amazon Best Sellers lists (https://www.amazon.com/gp/bestsellers/2025/books)
* **Time range:** 2024–2025 (with initial exploration including 2023)
* **Collection method:** Manual extraction of the top 100 bestselling books per year
* **Data storage:** Consolidated into a structured Excel file for analysis
* **Key features:** Title, Author, Number of Reviews, Rating, Price, Year
* **Scope:** Cross-sectional and time-based comparison of bestseller performance

**Limitations:**:

* Manual data collection may introduce inconsistencies
* Bestseller lists reflect Amazon-specific consumer behavior
* Missing or inconsistent data for certain years (e.g., 2023)


---

## **Data Cleaning & Preparation**:

The raw dataset required several cleaning and preprocessing steps to ensure consistency and reliability before analysis.

- **Standardization of book titles:**  
  Book titles were normalized by removing additional descriptors (e.g., editions, subtitles in parentheses) and standardizing text formatting (case, spacing). This was necessary to correctly aggregate duplicate entries of the same title.

- **Handling duplicates:**  
  Multiple entries of the same book across years and editions were consolidated to avoid fragmentation in the analysis and to ensure accurate comparisons.

- **Data type consistency:**  
  Numerical fields such as *Number of Reviews*, *Rating*, and *Price* were converted to appropriate numeric formats to enable aggregation and effective statistical analysis.

- **Missing values treatment:**  
  Missing or incomplete values were addressed where possible,(not always). Records with significant inconsistencies were either corrected or excluded from specific analyses to maintain data integrity.

- **Year filtering:**  
  The dataset was segmented by year (2023–2025). Due to too many inconsistencies and incomplete data in 2023, the final analysis focuses primarily on 2024 and 2025 to ensure comparability.

- **Feature preparation:**  
  Additional derived metrics (e.g., Popularity Score) were created by combining relevant variables such as number of reviews, rating, and frequency of appearance to better capture overall book performance.

---

## **Methodology**:

*The analysis followed a structured data-driven approach combining preprocessing, aggregation, and exploratory analysis. After cleaning and standardizing the dataset, records were grouped by key dimensions such as *Book Title* and *Author* to evaluate performance across years.

*Exploratory Data Analysis (EDA) was performed to understand distributions and identify patterns in ratings, review counts, pricing, and title frequency. Comparisons were then made across 2024 and 2025 to assess consistency and identify stable versus emerging bestsellers.

*To enable consistent ranking, a *Popularity Score* was derived by combining multiple performance indicators into a single metric. In parallel, normalization techniques were applied to standardize review counts and support fair visual comparison across titles and years.

*Finally, visualizations such as charts and heatmaps were used to surface trends and support interpretation of the results, enabling clear identification of top-performing books and authors.

* As a cherry on top a visually engaging PowerPoint presentation was created to communicate key findings clearly and effectively to stakeholders, enabling easy interpretation and supporting data-driven decision-making.

---

## Key Insights

- **Top Performers:** Titles such as *Fourth Wing*, *The Housemaid*, *Verity*, and *Onyx Storm* consistently dominate the ranking across the analyzed years.

- **Series-Driven Purchases:** The highest performing books are often part of the same series or share the same author, suggesting a strong repeat purchase pattern driven by reader loyalty and narrative continuity.

- **Stable Demand:** Minimal variation in performance across years indicates sustained popularity rather than short-lived trends.

- **Market Concentration:** A relatively small number of titles account for a disproportionate share of overall engagement, highlighting a concentrated demand structure.

- **Dual Track Market Value:** Series such as *ACOTAR* and *Fourth Wing* show signs of transitioning into “legacy status,” maintaining consistent but stabilizing demand. In contrast, *The Housemaid* represents a benchmark of both high popularity and strong consistency, positioning it as a key anchor title in the market.

- **Author Influence:** Author identity plays a pivotal role alongside individual titles. While future performance of new releases cannot be guaranteed, historical data suggests that established authors such as Freida McFadden and Rebecca Yarros are likely to continue driving strong demand in the near future.

---

## Final Recommendations:


Based on the analysis, several clear actions emerge for optimizing inventory and shelf strategy.

**Inventory and Shelf Strategy**


* Top-performing titles such as *Fourth Wing*, *The Housemaid*, *Verity*, and *Onyx Storm* should remain a priority in both stocking and in-store placement. These titles represent consistent demand and should be treated as core inventory, with sufficient stock depth to minimize the risk of stockouts. Where possible, all books within each series should be made available to fully capture repeat-purchase behavior.(very important)

* These titles should also be displayed in close proximity to one another, reinforcing discovery within the same series and author. This is particularly relevant for high-performing genres such as "romantasy," which show sustained popularity and strong cross title engagement. Grouping similar books together can improve visibility and support cross selling of related high ROI titles.

**The Repeat Purchase Pattern:**


* The analysis highlights a very clear repeat purchase pattern: readers who engage with one title in a series are highly likely to continue with subsequent installments and explore additional works by the same author. Retail strategies should therefore leverage this behavior by aligning shelf organization with series, authors, and thematic similarity, effectively guiding customers along a natural progression of discovery.

<img width="1536" height="1024" alt="IMG_3382" src="https://github.com/user-attachments/assets/815b1947-718c-4322-b3b4-537cab768d9a" />


**From an operational perspective:**


* Inventory allocation should reflect a structured, multi-levelled approach. Established bestsellers should receive higher inventory allocation and prominent placement, while secondary titles within the same ecosystem can support discovery and add breadth. New or emerging releases from already successful authors should be closely monitored and quickly incorporated into inventory, as they are likely to benefit from existing demand and brand recognition.

In conclusion, it is of vital important to continuously track new releases and emerging trends, as shifts in consumer preference can introduce new high performing titles. However, the current data (2024–2025) shows strong consistency among top performers, suggesting that established titles and authors will continue to anchor demand in the near term.

Overall, the findings support a strategy centered on prioritizing proven high demand titles, structuring shelves around series and authors, and maintaining flexibility to respond quickly to new successful releases. 

---

## **Limitations of the Analysis**

- **Data source scope:** The dataset is based on Amazon’s Top 100 Bestsellers list and does not represent the entire book market or all consumer segments.

- **Selection bias:** Bestseller lists inherently focus on high-performing titles, which may overrepresent popular genres and underrepresent niche or emerging categories.

- **Data consistency issues:** Some inconsistencies were identified in earlier years (notably 2023), including missing values and irregularities, which limited their reliability and led to a focus on 2024–2025.

- **Title standardization assumptions:** Book titles were cleaned and standardized to merge variants (e.g., subtitles and special editions). While necessary, this may introduce minor aggregation approximations.

- **Proxy metrics for demand:** Metrics such as number of reviews and ratings are used as proxies for popularity and demand, but they do not perfectly measure actual sales volume.

- **Lack of external factors:** The analysis does not account for external influences such as marketing campaigns, seasonal effects, pricing strategies over time, or publisher promotions.

- **Time window limitation:** The analysis focuses on recent years (2023, 2024–2025), which may not fully capture long-term historical trends or future shifts in reader preferences.

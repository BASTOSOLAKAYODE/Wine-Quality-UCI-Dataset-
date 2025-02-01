# Project Background

## About the Company
The company, **VinoAnalytics**, is a leading player in the wine industry, specializing in the production and distribution of high-quality red and white wines. With over **20 years of experience**, VinoAnalytics has built a reputation for delivering premium wines to both domestic and international markets. The company operates on a **direct-to-consumer (DTC) business model**, leveraging online sales platforms and partnerships with luxury retailers to reach its customers.

### Key Business Metrics
- **Revenue Growth**: Year-over-year revenue growth is a critical metric, driven by sales of premium wines.
- **Customer Satisfaction**: Measured through wine ratings and customer feedback, aiming for an average quality score of 7+.
- **Market Share**: The company aims to increase its market share by 5% annually through targeted marketing and product improvements.

## Project Overview
As a **Data Analyst** at VinoAnalytics, my role is to analyze the company’s wine quality data to uncover insights that can drive business decisions. This project focuses on understanding the factors that influence wine quality and providing actionable recommendations to improve product offerings and customer satisfaction.

### Key Areas of Analysis
1. **Category 1: Wine Quality by Type (Red vs. White)**
   - Analyze the differences in quality between red and white wines.
   - Identify which type of wine performs better in terms of customer ratings.

2. **Category 2: Alcohol Content and Quality**
   - Investigate the relationship between alcohol content and wine quality.
   - Determine if higher alcohol content leads to better ratings.

3. **Category 3: Sweetness (Residual Sugar) and Quality**
   - Explore whether sweeter wines (higher residual sugar) receive better ratings.
   - Assess the impact of sweetness on customer preferences.

4. **Category 4: Acidity Levels and Quality**
   - Examine the role of acidity (fixed acidity, volatile acidity, citric acid, pH) in determining wine quality.
   - Identify the optimal acidity levels for high-quality wines.

### Data Sources and Tools
- **Dataset**: The analysis is based on a dataset containing physicochemical properties and quality ratings for 5,320 red and white wines.
- **SQL Queries**: The data was inspected and cleaned using SQL. The queries can be found [here](#) (link to SQL queries).
- **Tableau Dashboard**: An interactive dashboard was created to visualize sales trends and wine quality metrics. Explore it [here](#) (link to Tableau dashboard).


# Data Structure & Initial Checks

The companies main database structure as seen below consists of four tables: table1, table2, table3, table4, with a total row count of X records. A description of each table is as follows:
- **Table 2:**
- **Table 3:**
- **Table 4:**
- **Table 5:**

[Entity Relationship Diagram here]



# Executive Summary

### Overview of Findings
This analysis identifies key drivers of wine quality and provides actionable insights to enhance product offerings and customer satisfaction. The three most important findings are:
1. **White wines outperform red wines** in quality ratings, with an average score of 5.85 compared to 5.62.
2. **Alcohol content is a strong predictor of quality**, with higher alcohol levels consistently associated with better ratings.
3. **Acidity levels significantly impact quality**, with optimal levels of fixed acidity and citric acid leading to higher scores, while volatile acidity should be minimized.

These insights can guide strategic decisions in production, marketing, and product development to improve customer satisfaction and drive revenue growth.

[Visualization, including a graph of overall trends or snapshot of a dashboard]



# Insights Deep Dive
### Category 1:

* **Main insight 1.** More detail about the supporting analysis about this insight, including time frames, quantitative values, and observations about trends.
  
* **Main insight 2.** More detail about the supporting analysis about this insight, including time frames, quantitative values, and observations about trends.
  
* **Main insight 3.** More detail about the supporting analysis about this insight, including time frames, quantitative values, and observations about trends.
  
* **Main insight 4.** More detail about the supporting analysis about this insight, including time frames, quantitative values, and observations about trends.

[Visualization specific to category 1]


# Insights and Recommendations
The analysis revealed several key insights:
1. **White wines** have significantly higher quality ratings than red wines, with an average score of 5.85 compared to 5.62.
2. **Alcohol content** is a strong predictor of wine quality, with a moderate positive correlation (0.47).
3. **Residual sugar** has no clear relationship with quality, suggesting that sweetness alone is not a key driver of customer satisfaction.
4. **Acidity levels** play a crucial role in wine quality, with higher fixed acidity and citric acid associated with better ratings.

# Recommendations
1. **Focus on White Wines**: Increase production and marketing efforts for white wines, as they consistently receive higher ratings.
2. **Optimize Alcohol Content**: Aim for wines with higher alcohol content to improve quality ratings.
3. **Monitor Acidity Levels**: Maintain optimal acidity levels (higher fixed acidity, lower volatile acidity) to enhance wine quality.
4. **Explore Customer Preferences**: Conduct surveys to better understand customer preferences for sweetness and other flavor profiles.
  


# Assumptions and Caveats:

Throughout the analysis, multiple assumptions were made to manage challenges with the data. These assumptions and caveats are noted below:

* Assumption 1 (ex: missing country records were for customers based in the US, and were re-coded to be US citizens)
  
* Assumption 1 (ex: data for December 2021 was missing - this was imputed using a combination of historical trends and December 2020 data)
  
* Assumption 1 (ex: because 3% of the refund date column contained non-sensical dates, these were excluded from the analysis)

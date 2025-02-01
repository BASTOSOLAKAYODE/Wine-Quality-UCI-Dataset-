# Project Background

## About the Company
The company, **Vinho Verde**, is a leading player in the wine industry, specializing in the production and distribution of high-quality red and white wines. With over **20 years of experience**, Vinho Verde has built a reputation for delivering premium wines to both domestic and international markets. The company operates on a **direct-to-consumer (DTC) business model**, leveraging online sales platforms and partnerships with luxury retailers to reach its customers.

### Key Business Metrics
- **Revenue Growth**: Year-over-year revenue growth is a critical metric, driven by sales of premium wines.
- **Customer Satisfaction**: Measured through wine ratings and customer feedback, aiming for an average quality score of 7+.
- **Market Share**: The company aims to increase its market share by 5% annually through targeted marketing and product improvements.

## Project Overview
This project focuses on understanding the factors that influence wine quality and providing actionable recommendations to improve product offerings and customer satisfaction.

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

The company's main database structure consists of four tables: `wine_data`, `customer_data`, `sales_data`, and `quality_metrics`, with a total row count of **5,320 records**. A description of each table is as follows:

- **Table 1: `wine_data`**
  - Contains physicochemical properties of wines, such as `fixed_acidity`, `volatile_acidity`, `citric_acid`, `residual_sugar`, `chlorides`, `free_sulfur_dioxide`, `total_sulfur_dioxide`, `density`, `pH`, `sulphates`, `alcohol`, and `color`.
  - **Primary Key**: `wine_id`
  - **Rows**: 5,320

- **Table 2: `customer_data`**
  - Stores customer information, including `customer_id`, `name`, `email`, `region`, and `preferred_wine_type`.
  - **Primary Key**: `customer_id`
  - **Rows**: 10,000

- **Table 3: `sales_data`**
  - Records sales transactions, including `transaction_id`, `wine_id`, `customer_id`, `sale_date`, `quantity`, and `revenue`.
  - **Primary Key**: `transaction_id`
  - **Rows**: 15,000

- **Table 4: `quality_metrics`**
  - Tracks quality ratings and feedback for each wine, including `wine_id`, `quality_score`, and `customer_feedback`.
  - **Primary Key**: `wine_id`
  - **Rows**: 5,320

[Entity Relationship Diagram here]


## Initial Data Checks
1. **Missing Values**:
   - Missing values in the `color` column were assumed to represent white wines and were re-coded accordingly.
   - Outliers in `residual_sugar` were excluded to ensure data quality.

2. **Data Types**:
   - All numerical columns were verified to be of type `float` or `int`.
   - Categorical columns (`color`, `region`, etc.) were converted to type `category`.

3. **Duplicates**:
   - No duplicate records were found in the `wine_data` or `quality_metrics` tables.

4. **Consistency**:
   - The `wine_id` column was used to join `wine_data` and `quality_metrics`, ensuring consistency across tables.

# GitHub Repository Structure
```
wine-quality-analysis/
├── data/
│   ├── raw/                      # Original, unprocessed data files
│   │   └── wine_data.csv
│   ├── processed/                # Cleaned and processed data files
│   │   └── cleaned_wine_data.csv
│   └── README.md                 # Description of data sources and structure
│
├── notebooks/
│   ├── 01_data_cleaning.ipynb    # Data cleaning and preprocessing
│   ├── 02_eda.ipynb             # Exploratory Data Analysis
│   ├── 03_statistical_analysis.ipynb  # Statistical tests and insights
│   ├── 04_model_building.ipynb   # Machine learning model development
│   └── README.md                 # Overview of notebooks
│
├── scripts/
│   ├── data_cleaning.py         # Python script for data cleaning
│   ├── model_training.py        # Python script for model training
│   └── README.md                # Description of scripts
│
├── models/
│   └── wine_quality_predictor.pkl  # Saved machine learning model
│
├── reports/
│   ├── figures/                 # Visualizations and plots
│   │   └── quality_distribution.png
│   └── final_report.pdf        # Final analysis report
│
├── .gitignore                   # Files and folders to ignore
├── requirements.txt             # Python dependencies
└── README.md                    # Project overview and instructions
```
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
  

# Assumptions and Caveats

Throughout the analysis, multiple assumptions were made to manage challenges with the data. These assumptions and caveats are noted below:

1. **Assumption 1**: Missing values in the `color` column (indicating wine type) were assumed to represent **white wines**, as they constitute the majority of the dataset. These records were re-coded as "white" to ensure completeness.

2. **Assumption 2**: Outliers in the `residual_sugar` column (e.g., extremely high values) were assumed to be data entry errors and were excluded from the analysis to avoid skewing results.

3. **Assumption 3**: The `quality` column, which contains integer scores from 3 to 9, was treated as a continuous variable for regression analysis, despite being ordinal in nature. This assumption was made to simplify modeling and interpretation.

4. **Caveat 1**: The dataset does not include information on external factors such as **vintage year**, **region**, or **storage conditions**, which could significantly impact wine quality. As a result, the analysis focuses solely on physicochemical properties.

5. **Caveat 2**: The analysis assumes that the dataset is representative of the broader wine market. However, the data may be biased toward specific regions or production methods, limiting generalizability.

6. **Caveat 3**: The machine learning model's performance (R² = 0.52) indicates moderate predictive power. While useful, the model may not capture all nuances of wine quality, and predictions should be interpreted with caution.

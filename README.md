# Analysis of the Relationship Between TCMB Interest & Inflation Rates and Google Search Trends

## Overview
This project aims to analyze the relationship between the monthly interest and inflation rates published by the Central Bank of the Republic of Turkey (TCMB) and the frequency of Google searches for the terms **inflation, interest rate, euro, and dollar**. By examining search trends over the past five years, this study seeks to understand how economic concerns influence public interest in these topics.

## Hypotheses
This study tests the following hypotheses:

1. **Interest Rate Changes and Search Trends:** Increases or decreases in TCMB’s interest rates correlate with fluctuations in search volumes for "faiz" (interest rate) and "dollar/euro."
2. **Inflation and Public Interest:** Rising inflation leads to increased searches for "enflasyon" (inflation), as the public seeks more information about its impact on daily life.

## Table of Contents
- [Motivation](#motivation)
- [Project Goal](#project-goal)
- [Data Sources and Preprocessing](#data-sources-and-preprocessing)
- [Data Analysis](#data-analysis)
- [Findings](#findings)
  - [Hypothesis Testing](#hypothesis-testing)
  - [Machine Learning Techniques](#machine-learning-techniques)
- [Limitations and Future Work](#limitations-and-future-work)

## Motivation
Macroeconomic indicators such as interest rates and inflation significantly affect a country’s financial environment. Public perception and reaction to economic changes can be observed through online search trends. By studying the relationship between TCMB’s monetary policies and public interest in financial terms, this project aims to:

- Identify correlations between monetary policies and public concern about inflation and exchange rates.
- Understand how interest rate adjustments influence search behaviors.
- Examine whether financial uncertainty is reflected in search trends for "dollar" and "euro."
- Provide insights into how digital data can be used to track economic sentiment.

## Project Goal
The primary goal of this project is to analyze the interaction between **TCMB’s interest and inflation rates** and **Google search trends for economic terms** over the past five years. By using monthly data, this study seeks to uncover potential patterns and relationships that indicate public reaction to economic changes.

## Data Sources and Preprocessing
The dataset for this study will be collected from the following sources:

- **TCMB Data:** Monthly interest rate and inflation statistics.
- **Google Trends Data:** Monthly search frequency of the terms **inflation, interest rate, euro, and dollar.**

### Preprocessing Steps:
1. **Data Cleaning:** Ensuring consistency between different data sources.
2. **Time Alignment:** Synchronizing economic data and Google Trends data by month.
3. **Normalization:** Adjusting search volumes to account for overall changes in Google search activity.
4. **Additional Columns:** New columns were created for:
   - **Inflation Rate Difference**: The difference between the current month’s inflation rate and the previous month’s inflation rate.
   - **Interest Rate Change**: The change in the TCMB interest rate compared to the previous month.

## Data Analysis
In this section, the analysis focuses on exploring relationships between the **TCMB data** and **Google search trends**. The main techniques used for this analysis include:

### Correlation Analysis:
Spearman’s rank correlation was computed to examine how changes in **interest rates** and **inflation rates** correlate with fluctuations in Google search volumes for terms like **"faiz"** and **"enflasyon"**.

### Hypothesis Testing:
Two hypotheses were tested:
1. **Interest Rate Changes and Search Trends**: Whether changes in TCMB's interest rate have a noticeable impact on public search behavior related to financial terms.
2. **Inflation and Public Interest**: Whether inflation correlates with an increase in searches for "enflasyon" and related terms.

**Results from Hypothesis Testing**:
- **Interest Rate Correlation**: A moderate positive correlation was found between TCMB interest rate changes and searches for "faiz" (interest rate).
- **Inflation and Search Trends**: A strong positive correlation was found between the increase in inflation rates and searches for "enflasyon" (inflation), confirming that public concern about inflation drives interest in related terms.

## Findings
- Public interest in financial topics such as inflation and interest rates is highly reactive to changes in TCMB's economic policies.
- The regression model suggests that interest rate changes are a significant predictor of increases in search volumes related to "faiz" (interest rate).
- Google Trends data can serve as a useful proxy for measuring public sentiment regarding economic conditions.

## Limitations and Future Work

### Limitations:
- The analysis assumes that search volume is a direct reflection of public concern, but other factors may influence search behavior (e.g., media coverage, political events).
- The time span of five years may not capture long-term economic trends.


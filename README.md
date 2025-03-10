# DSA210-Term-Project

I am a student from Sabancı University, Yağmur Geçim, and this is my DSA210 term project. The aim of this project is to analyze the interaction between digital sentiment—captured through Google Trends search data—and key macroeconomic indicators in Turkey over the last 5 years.

These two hypotheses will be tested:

**First hypothesis:** Increased search interest for economic terms (e.g., "inflation" and "interest") correlates with higher consumer price index values and shifts in credit interest rates.  
**Second hypothesis:** Changes in digital sentiment, as measured by search trends for terms like "euro" and "dollar," precede movements in macroeconomic indicators, indicating potential early warning signals.

---

## Contents

- [Motivation](#motivation)
- [Project Goal](#project-goal)
- [Data Sources and Preprocessing](#data-sources-and-preprocessing)
- [Data Analysis](#data-analysis)
- [Findings](#findings)
- [Hypothesis Testing](#hypothesis-testing)
- [Machine Learning Techniques](#machine-learning-techniques)
- [Limitations and Future Work](#limitations-and-future-work)

---

## Motivation

Economic sentiment and policy shifts are increasingly mirrored in digital behavior. Understanding how online search trends relate to traditional economic indicators can provide valuable insights into market dynamics and serve as an early warning system. By analyzing data from Google Trends alongside official data on the Consumer Price Index (CPI) and Average Weighted Credit Interest Rates, this project aims to explore the potential predictive power of digital sentiment on macroeconomic performance.

---

## Project Goal

The goal of this project is to uncover and quantify the relationship between digital sentiment—as reflected in search trends for "euro", "dollar", "interest", and "inflation"—and key economic indicators such as the CPI (2003=100) and bank credit interest rates. Through this analysis, I aim to:
- Identify correlations and time-lagged effects between search trends and economic indicators.
- Determine if shifts in digital sentiment can serve as a precursor to changes in macroeconomic conditions.
- Provide insights that could support the development of early warning systems for economic policy makers.

---

## Data Sources and Preprocessing

### Data Sources
1. **Google Trends Data:**  
   - Terms: "euro", "dollar", "interest", "inflation"  
   - Time Frame: Last 5 years  
   - Data will be collected via the Google Trends API or manual downloads.

2. **Consumer Price Index (CPI) (2003=100):**  
   - Sourced from the Turkish Statistical Institute (TÜİK).  
   - [TÜİK Data Portal](https://data.tuik.gov.tr/)

3. **Average Weighted Credit Interest Rates:**  
   - Sourced from the Central Bank of the Republic of Turkey (TCMB).  
   - [TCMB Statistics](https://www.tcmb.gov.tr/wps/wcm/connect/tcmb+tr/tcmb+tr/main+menu/istatistikler)

### Preprocessing Steps
- **Data Cleaning:**  
  Remove or correct any missing or inconsistent data points.
  
- **Time Series Alignment:**  
  Ensure that the time intervals for Google Trends data and economic indicators match (e.g., monthly data).

- **Data Merging:**  
  Combine the datasets into a single time-indexed dataset for comprehensive analysis.







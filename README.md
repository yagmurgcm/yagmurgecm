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
  
<img width="627" alt="Ekran Resmi 2025-04-25 19 45 32" src="https://github.com/user-attachments/assets/2f784bd7-f50e-49f0-8b51-93b6c03382ad" />
  
*The scatter plot illustrates a positive relationship between TCMB's interest rate and the search volume for "faiz" (interest rate) on Google Trends. The Spearman correlation coefficient of 0.606 suggests a moderate positive correlation, indicating that as TCMB's interest rate increases, the public shows increased interest in searching for "faiz" on Google. The p-value of 0.0 confirms that this correlation is statistically significant, meaning the observed relationship is not due to chance. This finding implies that changes in TCMB's monetary policy, particularly interest rate adjustments, are likely influencing public interest and concern about interest rates, as reflected in search behaviors.

<img width="632" alt="Ekran Resmi 2025-04-25 19 45 40" src="https://github.com/user-attachments/assets/91f0c81a-ac6c-436c-8f8d-ca79f3edb677" />

*The scatter plot reveals a negative relationship between TCMB's interest rate and the Google search volume for "dolar" (dollar). The Spearman correlation coefficient of -0.453 indicates a moderate negative correlation, meaning as TCMB's interest rate increases, the public's interest in searching for "dolar" decreases. The p-value of 0.00031 confirms that this correlation is statistically significant, allowing us to reject the null hypothesis (H₀), which states there is no correlation. This suggests that as TCMB raises interest rates, people may be less concerned with or searching for the dollar, possibly due to expectations of reduced currency volatility or a stable exchange rate resulting from the rate increase.

<img width="636" alt="Ekran Resmi 2025-04-25 19 45 46" src="https://github.com/user-attachments/assets/4658c5e4-93ec-4190-9c51-af12136a5619" />
  
*The scatter plot shows the relationship between TCMB's interest rate and Google search volumes for "euro". The Spearman correlation coefficient of 0.187 indicates a very weak positive correlation. However, the p-value of 0.15547 is greater than the typical significance threshold of 0.05, meaning the correlation is not statistically significant. As a result, we fail to reject the null hypothesis, suggesting that there is no meaningful relationship between TCMB's interest rate and the public's interest in searching for "euro." This implies that changes in interest rates do not have a notable impact on search volumes for the term "euro."
  
- **Inflation and Search Trends**: A strong positive correlation was found between the increase in inflation rates and searches for "enflasyon" (inflation), confirming that public concern about inflation drives interest in related terms.

<img width="988" alt="Ekran Resmi 2025-04-25 19 45 55" src="https://github.com/user-attachments/assets/db928ce8-0027-4922-b4b8-9dd295d4dee3" />

*The scatter plot shows the relationship between TCMB inflation rate (annual percentage change) and the Google search trend for "enflasyon" (inflation). The Spearman correlation coefficient of 0.66 suggests a moderate positive correlation, indicating that as TCMB's inflation rate increases, public interest in searching for "enflasyon" also rises. The p-value of 0.0 confirms the correlation is statistically significant, allowing us to reject the null hypothesis (H₀), meaning there is a significant relationship between inflation rates and public search behavior regarding inflation. This indicates that as inflation rises, people tend to search more for information about inflation, reflecting a higher public concern about economic conditions.

## Machine Learning
**-TCMB Interest Rates vs Interest Rates Search Trends**

<img width="658" alt="Ekran Resmi 2025-05-18 17 28 54" src="https://github.com/user-attachments/assets/07703597-fc9f-4e9a-8937-78dd553c11ab" />

The graph above shows the Random Forest model’s predictions of Turkey’s central bank interest rate based solely on Google search trends for "interest".
With an R² score of 0.76, the model demonstrates a strong fit between public search behavior and actual interest rates, indicating that search data can serve as a valuable predictor even in small datasets.


**-TCMB Inflation Rates vs Inflation Rates Search Trends**

<img width="667" alt="Ekran Resmi 2025-05-18 17 31 00" src="https://github.com/user-attachments/assets/eb9de26b-2940-40a4-a4ff-a18f94988111" />

The graph displays the Random Forest model's prediction of Turkey’s official inflation rate based solely on Google search trends related to inflation.
Although the data shows some variability, the model achieved a solid R² score of 0.44, indicating that search behavior still holds meaningful predictive power for inflation rates.



## Findings
- Public interest in financial topics such as inflation and interest rates is highly reactive to changes in TCMB's economic policies.
- The regression model suggests that interest rate changes are a significant predictor of increases in search volumes related to "faiz" (interest rate).
- Google Trends data can serve as a useful proxy for measuring public sentiment regarding economic conditions.

## Limitations and Future Work

### Limitations:
- The analysis assumes that search volume is a direct reflection of public concern, but other factors may influence search behavior (e.g., media coverage, political events).
- The time span of five years may not capture long-term economic trends.



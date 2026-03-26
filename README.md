# 🇷🇼 Economic Trends in Rwanda (2001–2024)

## Project Overview

This project analyzes the macroeconomic performance of Rwanda between 2001 and 2024 using World Bank World Development Indicators (WDI).

The analysis applies data cleaning, exploratory data analysis (EDA), correlation analysis, and regression modeling in **R** to examine trends in GDP growth, inflation, trade, and unemployment.

The objective is to demonstrate **data analytics, visualization, and econometric modeling skills** while building a reproducible workflow for economic analysis.

---

##  Objectives

* Analyze trends in GDP growth over time
* Assess inflation dynamics and stability
* Examine trade integration into the global economy
* Evaluate relationships between key macroeconomic variables

---

## Tools & Libraries

* **Data Handling:** dplyr, tidyr, readr
* **Visualization:** ggplot2, ggcorrplot, corrplot
* **Modeling & Diagnostics:** lm(), car (VIF analysis)
* **Reproducibility:** RMarkdown

---

## Dataset

* **Source:** World Bank World Development Indicators
* **Country:** Rwanda
* **Period:** 2001–2024

### Key Indicators:

* GDP (constant 2015 US$)
* GDP growth rate (%)
* Inflation (%)
* Population
* Unemployment rate (%)
* Exports & Imports (% of GDP)
* Trade (% of GDP)
* Government expenditure (% of GDP)
* Tax revenue (% of GDP)
* Current account balance (% of GDP)
* Foreign direct investment (% of GDP)
* Exchange rate
* Gross capital formation (% of GDP)

---

## Workflow

### 1. Data Cleaning & Preparation

* Converted missing values (“..”) to NA
* Removed unnecessary columns
* Renamed variables for clarity
* Filtered Rwanda data (2001–2024)

---

### 2. Exploratory Data Analysis (EDA)

* GDP growth shows **relative stability with fluctuations**, rather than a consistent upward trend
* Clear economic disruptions during:

  * 2008 global financial crisis
  * COVID-19 pandemic (2020)
* Trade (% of GDP) shows a **strong upward trend**, indicating increasing global integration

---

### 3. Correlation Analysis

* Weak relationships between GDP growth and:

  * Inflation
  * Unemployment
  * Trade variables
* Strong positive correlation between **exports and imports**, reflecting interconnected trade dynamics

---

### 4. Regression Modeling

* Initial model:
  GDP growth ~ Inflation + Exports + Imports + Unemployment

* Multicollinearity detected:

  * High correlation between exports and imports (VIF > 6)

* Revised model:
  GDP growth ~ Inflation + Exports + Unemployment

* **Result:**

  * Low explanatory power (~6%)
  * No statistically significant predictors

 Interpretation: Rwanda’s economic growth is influenced more by **structural and external factors** than by short-term macroeconomic indicators.

---

### 5. Trend Comparison

* GDP growth: stable but volatile
* Inflation: highly variable over time
* Trade: steadily increasing

These trends highlight:

* Economic resilience
* Growing globalization
* Ongoing macroeconomic challenges

---

##  Key Insights

* Rwanda’s growth is **resilient but sensitive to external shocks**
* Inflation exhibits **volatility rather than sustained stability**
* Trade expansion reflects **increasing global economic integration**
* Economic growth is **not strongly explained by simple macro variables alone**

---

## Limitations

* Small sample size (2001–2024)
* Omitted variable bias
* No causal inference (correlation ≠ causation)
* Limited time-series modeling

---

##  Skills Demonstrated

* Data cleaning and transformation in R
* Data visualization and storytelling
* Statistical analysis (correlation & regression)
* Multicollinearity diagnostics (VIF)
* Economic interpretation of data
* Reproducible research workflow

---

## How to Run

1. Clone the repository:
 
2. Open the RMarkdown file in RStudio

3. Install required packages:
   install.packages(c("dplyr","ggplot2","ggcorrplot","corrplot","car","tidyr","readr"))

4. Knit to PDF or HTML

---

##  Future Improvements

* Time-series modeling (ARIMA, VAR)
* Interactive dashboards (Shiny / Plotly)
* Cross-country comparison (e.g., East African economies)
* Automated data updates via World Bank API

---

##  Author

**Benjamin Bahizi Sebujisho**
Data Analyst | Economist | R Programmer

🔗 LinkedIn: https://www.linkedin.com/in/bahizi-sebujisho-benjamin-897b062a6/


🔗 GitHub: https://github.com/bahizibenjmain

---

## 💡 Project Value

This project demonstrates the ability to transform raw economic data into meaningful insights using statistical and analytical tools—skills essential for roles in **data analysis, development economics, and policy research**.

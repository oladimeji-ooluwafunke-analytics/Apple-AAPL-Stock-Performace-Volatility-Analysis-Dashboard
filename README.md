# 📊 Apple (AAPL) Stock Performance & Volatility Analysis Dashboard
## 📌 Project Description

This project presents an interactive **Power BI dashboard designed to analyze the historical performance of Apple Inc. (AAPL)** using financial market data and product revenue metrics. The analysis focuses on understanding stock price behavior, technical indicators, volatility patterns, and the relationship between company revenue and stock performance.

The dashboard integrates multiple analytical perspectives including **stock performance trends, risk indicators, quarterly performance analysis, and revenue vs stock performace**. By combining financial data with structured analytics and visualization techniques, the project demonstrates how business intelligence tools can transform raw financial data into meaningful insights that support strategic decision-making.

This project highlights practical applications of **data cleaning, data modeling, DAX calculations, and interactive dashboard development** in a financial analytics context.

## 🎯 Business Objective

Financial markets generate large volumes of time-series data that require structured analysis to extract meaningful insights.

The objective of this project is to:

* Analyze Apple’s historical stock price performance
* Identify risk patterns using technical indicators
* Evaluate quarterly performance trends
* Analyze volatility across time periods
* Explore the relationship between product revenue and stock market behavior
* Present insights through an interactive Power BI dashboard

The dashboard enables analysts, investors, and decision-makers to **monitor stock performance, assess market risk, and explore financial trends in a clear and structured manner.**

## 🛠 Tools Use

The following tools and technologies were used to build this project:

* Power BI Desktop– Dashboard development and visualization
* Power Query Editor – Data cleaning and transformation
* DAX (Data Analysis Expressions) – Custom measures and calculations
* Excel Dataset– Source data for stock and revenue metrics
* Data Modeling – Building relationships between datasets

 ## 📂 Dataset Description

The analysis utilizes structured datasets containing both **daily stock market data and quarterly performance metrics**.

### Daily Stock Dataset

This dataset includes detailed trading records such as:

* Date
* Opening price
* High price
* Low price
* Closing price
* Trading volume
* Daily return
* RSI (Relative Strength Index)
* Volatility metrics
* Fiscal year and quarter identifiers

This dataset enables **granular analysis of daily stock behavior and technical indicators.**

---

### Quarterly Performance Dataset

This dataset contains aggregated quarterly metrics including:

* Fiscal year
* Fiscal quarter
* Quarterly return percentage
* Average volatility
* Revenue metrics by product

The quarterly dataset allows the analysis to focus on **long-term trends and seasonal financial patterns.

##  Data Cleaning & Preparation
Before building the dashboard, the dataset was cleaned and transformed using **Power Query Editor** to ensure data quality and analytical accuracy.

Key preparation steps included:

* Removing unnecessary columns that were not relevant for analysis
* Standardizing data types for numerical and date fields
* Creating a **Year-Quarter field** for easier time-based analysis
* Verifying numeric columns used in DAX calculations
* Ensuring consistency between fiscal year and fiscal quarter fields
* Validating aggregated metrics used for quarterly analysis

These steps ensured that the data model remained **efficient, accurate, and optimized for dashboard performance.

##  Data Modeling
A structured data model was created to enable efficient analysis across multiple datasets.

Key modeling steps included:

* Linking daily stock data with quarterly summary data
* Creating relationships using fiscal period identifiers
* Ensuring proper aggregation for quarterly metrics
* Structuring the model to support dynamic filtering and cross-visual interaction

A well-designed data model ensures that all visuals respond correctly to slicers and filters while maintaining high performance.

##  DAX Measures Implemented
Several calculated measures were implemented using DAX to support dynamic analysis and visualization.

Average Close Price = AVERAGE(aapl_master_enriched[close])
Average Daily Return = AVERAGE(aapl_master_enriched[daily_return])

Average RSI = AVERAGE(aapl_master_enriched[rsi_14])

Average Volatility = AVERAGE(aapl_quarterly_summary[volatility_20d_mean])

Quarterly Return % = AVERAGE(aapl_quarterly_summary[quarterly_return_pct])

These measures allow Power BI to dynamically calculate metrics based on user selections and dashboard filters.


## 📊 Dashboard Pages & Visualizations

### 📈 Page 1 — Stock Performance Overview

## Purpose
This page provides a high-level view of Apple’s stock performance and market returns.

### Visualizations

## KPI Cards
    * Display key performance indicators summarizing stock behavior.

## Year Slicer**
    * Enables users to filter the analysis by specific years.

## Line Chart 
    * Average Yearly Closing Price

* Displays long-term trends in Apple’s stock price.
 ## Line Chart — Average Daily Return**
    * Shows fluctuations in daily stock returns across time.

### Insights Provided

This page helps users quickly identify :
   * overall price growth trends and return fluctuations,
   * providing a strong foundation for further analysis.

### 📉 Page 2 — Risk & Technical Indicators (RSI) Analysis
### Purpose

This page focuses on analyzing **market risk and momentum indicators** using technical analysis metrics.

### Visualizations

**Gauge Chart — Average RSI**

* Displays the overall RSI level for the selected period.

**Table Visualization**

* Provides detailed values for RSI and other technical metrics.

**Line Chart — Date vs Volatility**

* Shows volatility trends across time.

**Line Chart — Date vs RSI**

* Displays how market momentum changes over time.

### Insights Provided

This page helps identify **periods of increased market risk and potential overbought or oversold conditions.

# 📊 Page 3 — Quarterly Performance Analysis
### Purpose

This page evaluates Apple’s performance from a **quarterly financial perspective**.

### Visualizations

**KPI Card — Quarterly Return**

* Displays the return percentage for the selected quarter.

**Table Visualization**

* Shows detailed quarterly performance metrics.

**Line Chart — Quarterly Return % vs Year Quarter**

* Displays performance trends across fiscal quarters.

**Line Chart — Average Volatility vs Year Quarter**

* Highlights volatility levels across different quarters.

### Insights Provided

This analysis reveals **quarter-to-quarter performance patterns and volatility fluctuations.

### 📊 Page 4 — Revenue Vs Stock Performance
### Purpose

This page explores how Apple’s **product revenue performance relates to stock market behavior.**

### Visualizations

**Pie Chart — Product Average Revenue**

* Displays revenue contribution by product category.

**Table Visualization**

* Provides detailed product revenue values.

**Stacked Column Chart — Product Revenue vs Year Quarter**

* Shows revenue trends for products across fiscal quarters.

### Insights Provided

This page helps analyze **how revenue distribution across products contributes to overall company performance and potential stock valuation.

#  Key Insights

* Apple’s stock demonstrates consistent long-term growth despite short-term volatility fluctuations.
* Periods of high volatility often correspond with increased market uncertainty.
* RSI analysis reveals momentum shifts that may signal potential market reversals.
* Quarterly analysis highlights fluctuations in returns and volatility across fiscal periods.
* Revenue analysis shows how product performance contributes to overall company growth.

---

# ✅ Recommendations

* Investors should monitor periods of elevated volatility before making major investment decisions.
* RSI indicators can support entry and exit strategies when combined with broader trend analysis.
* Price movements accompanied by strong trading volume often indicate stronger market participation.
* Portfolio diversification strategies may help mitigate risks during volatile market periods.
* Long-term investment decisions should prioritize sustained performance trends rather than short-term fluctuations.

---

#  Skills Demonstrated

This project demonstrates proficiency in:

* Data Cleaning and Transformation
* Data Modeling
* DAX Calculations
* Financial Data Analysis
* Interactive Dashboard Development
* Data Visualization and Storytelling
* Business Insight Communication

---

# 📷 Dashboard Preview
   ![Apple (AAPL) Dashboard](Apple%20(AAPL)%20dashboard%20image/Screenshot%202026-03-04%20063217.png)
   






# ⭐ Project Purpose

This project forms part of my **data analytics portfolio**, demonstrating how financial market data can be transformed into actionable insights through structured analysis and professional dashboard design.



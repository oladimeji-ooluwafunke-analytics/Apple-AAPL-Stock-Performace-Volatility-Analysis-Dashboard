# 📊 Apple (AAPL) Stock Performance & Volatility Analysis Dashboard
## 📌 Project Overview

This project presents an interactive **Power BI dashboard** designed to analyze Apple Inc. (AAPL) stock performance using historical market data. The objective of this analysis is to evaluate price behavior, trading activity, volatility patterns, and technical indicators across different fiscal periods to support data-driven investment insights.

The dashboard integrates both **daily trading data** and **quarterly aggregated metrics** to provide a comprehensive view of market performance while enabling trend monitoring, risk assessment, and performance comparison over time.

This project demonstrates practical applications of **data cleaning, transformation, data modeling, DAX calculations, and business-focused visualization design** within a financial analytics context.

## 🎯 Business Objective

Financial markets generate large volumes of time-series data that can be difficult to interpret without structured analytical tools.

The goal of this project is to:

* Analyze historical stock price performance
* Identify volatility and risk patterns
* Monitor trading volume behavior
* Evaluate technical indicators such as RSI
* Provide actionable insights for investment decision-making

## 🛠 Tools Use

* **Power BI Desktop**
* **Power Query (Data Cleaning & Transformation)**
* **DAX (Data Analysis Expressions)**
* Financial Market Dataset (AAPL Historical Data)
* Data Modeling & Relationship Management

 ## 📂 Dataset Description

The analysis utilizes two primary datasets:

### 1. Daily Stock Dataset (aapl_master_enriched)

Contains detailed trading information including:

* Date
* Open, High, Low, Close prices
* Trading Volume
* RSI (Relative Strength Index)
* 20-Day Volatility Metrics
* Fiscal Year & Quarter information

### 2. Quarterly Summary Dataset (aapl_quarterly_summary)

Pre-aggregated quarterly performance metrics including:

* Fiscal Year
* Fiscal Quarter
* Average Closing Price
* Mean Volatility
* Average Volume
* Quarterly Performance Indicators

Using quarterly aggregated data improves analytical efficiency and prevents unnecessary recalculation from daily records.

## 🧹 Data Cleaning & Preparation

Data transformation was performed using **Power Query Editor** to ensure analytical accuracy and model efficiency.

Key cleaning steps included:

* Removal of unnecessary or duplicate columns to reduce model complexity
* Standardization of column data types (Date, Text, Decimal Number)
* Handling inconsistent formatting across fiscal period fields
* Creation of a unified **Year-Quarter field** for time-based analysis
* Validation of numeric fields used for aggregation and DAX measures
Proper data preparation ensured reliable aggregation and accurate visual reporting.

## 🔗 Data Modeling

A structured data model was implemented following star-schema best practices.

* Daily and quarterly datasets were connected using fiscal period fields.
* Relationships were configured to enable synchronized filtering across visuals.
* Pre-aggregated quarterly metrics were prioritized for performance optimization.
* Redundant tables were excluded from active analysis to maintain model clarity.

Effective data modeling ensured accurate cross-table analysis and improved dashboard responsiveness.

## 📐 DAX Measures Implemented

The following measures were created to support analytical insights:

## 📐 DAX Measures Implemented

The following measures were created to support analytical insights:

DAX
Average Close Price = AVERAGE(aapl_master_enriched[close])

Total Volume = SUM(aapl_master_enriched[volume])

Average RSI = AVERAGE(aapl_master_enriched[rsi_14])

Average Volatility = 
AVERAGE(aapl_quarterly_summary[volatility_20d_mean])

These measures enable dynamic aggregation based on filters and slicer selections.

## 📊 Dashboard Pages & Visualizations

### 📈 Page 1 — Stock Performance Overview

**Purpose:** Monitor overall price behavior and trading activity.

Visuals include:

* Daily Reture Over Time (Line Chart)
* Close Price Over Time (Line Chart)
* Average Price / Total Volume KPI Cards
* Time/Year-based performance slicers

This page provides a high-level understanding of stock movement trends.

### 📉 Page 2 — Risk & Technical Indicators (RSI) Analysis

**Purpose:** Assess market momentum and potential reversal zones.

Visuals include:

* Average RSI Trend Over Time
* Sum of volatility_20d by Year
* Average RSI by Year
* Interactive filtering by fiscal period

Supports identification of overbought and oversold market conditions.

### 📊 Page 3 — Quarterly Performance Analysis

**Purpose:** Compare performance across fiscal quarters.

Visuals include:

* Average Quarterly Return
* Average 20-Day Volatility by Quarter
* Quarterly Return Performance
* Interactive slicers for trend exploration

Provides strategic performance evaluation across time periods.


### 📊 Page 4 — Revenue Vs Stock Performance

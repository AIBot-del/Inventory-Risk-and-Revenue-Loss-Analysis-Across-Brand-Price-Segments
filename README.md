# Brand Strategy & Inventory Risk Analysis

### ASOS E-commerce Dataset

## Executive Summary

This project analyzes ASOS product data to evaluate how brand pricing relates to stock availability and revenue loss due to stockouts. The analysis identifies key pricing segments where inventory inefficiencies lead to significant revenue leakage.

Findings show that inventory risk is not concentrated in premium products but is most significant in mid-priced, high-volume brands. These insights can be used to improve demand forecasting, stock allocation, and replenishment strategies.

---

## Problem Statement

Retail businesses often face revenue loss due to stockouts, but it is not always clear:

* Which price segments contribute most to stockout risk
* Whether higher-priced products are more operationally vulnerable
* Where inventory inefficiencies create the highest revenue leakage

This project addresses these questions using data-driven analysis.

---

## Objectives

* Analyze the relationship between product price and stockout rate
* Quantify revenue loss across brand segments
* Identify high-risk pricing zones contributing to inventory inefficiency
* Provide actionable insights for inventory optimization

---

## Dataset Overview

The dataset includes product-level ASOS data aggregated at brand level:

**Key variables:**

* Brand name
* Product price
* Stockout count (availability failure proxy)
* Estimated lost revenue
* Product frequency per brand

Only brands with more than 10 products were included to ensure statistical validity.

---

## Methodology

### 1. Data Aggregation (Brand-Level Analysis)

Data was grouped by brand to compute:

* Average price per brand
* Average stockout count
* Total lost revenue
* Product volume per brand

### 2. Data Cleaning & Filtering

Brands with low product counts (<10) were excluded to reduce bias and noise.

### 3. Feature Engineering

A normalized stockout rate was calculated:

Stockout Rate = Stockout_Count / Maximum Stockout_Count

This enabled comparability across brands.

### 4. Exploratory Data Analysis (EDA)

A scatter plot was used to analyze:

* Price vs Stockout Rate
* Revenue impact via bubble size

Thresholds were applied:

* £40 price boundary
* 0.4 stockout rate boundary

### 5. Risk Segmentation

Brands exceeding both thresholds were classified as high-risk and highlighted for further interpretation.

---

## Key Results

### 1. Mid-priced segment is the highest risk zone

Brands in the £25–£60 price range show the highest concentration of stockout activity combined with meaningful revenue loss.

### 2. Premium brands show lower operational risk

Higher-priced brands tend to have lower stockout rates, suggesting more controlled inventory management or lower demand volatility.

### 3. Low-priced products show extreme stockout behavior

Certain low-cost brands exhibit near-complete stockouts, indicating fast-moving demand and understocking risk.

### 4. Revenue loss is volume-driven, not price-driven

Mid-tier products contribute disproportionately to total revenue loss due to higher sales volume.

---

## Business Impact

This analysis identifies key opportunities for retail optimization:

* Reduce revenue leakage in mid-priced high-demand categories
* Improve forecasting accuracy for fast-moving SKUs
* Strengthen replenishment strategies for high-velocity products
* Optimize inventory allocation at a more granular (size/SKU) level
* Improve availability consistency for high-margin products

---

## Tools & Technologies

* Python (Pandas, NumPy)
* Matplotlib & Seaborn
* Data aggregation and feature engineering
* Exploratory Data Analysis (EDA)
* Business intelligence visualization techniques

---

## Key Takeaway

Inventory inefficiency is not driven by premium pricing but by mid-priced, high-demand segments where stock planning fails to match demand. This results in the highest hidden revenue loss.

---

## Outcome

The analysis provides a data-driven framework for:

* Identifying revenue leakage points
* Improving stock allocation decisions
* Supporting demand forecasting strategies
* Enhancing retail inventory efficiency

---

## Skills Demonstrated

* Data cleaning and preprocessing
* Aggregation and feature engineering
* Business-focused exploratory data analysis
* Data visualization and storytelling
* Retail analytics and inventory optimization
* Insight generation for decision-making

---

## Summary 

Identified mid-priced product segments as the primary source of revenue loss due to stockouts using brand-level pricing, availability, and revenue analysis on ASOS retail data.

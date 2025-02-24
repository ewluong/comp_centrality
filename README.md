# Assessing the Impact of Executive Diversity/Centrality on Firm Performance

**Project Sponsorship:** VANGUARD

---

## Overview

This project dives into how executive diversity and leadership centrality might influence firm performance. In today’s globalized and ever-changing market, understanding the nuances behind boardroom composition isn’t just academic—it could actually impact real-world investment decisions.

---

## Abstract

Our study explores the relationship between leadership diversity (covering ethnicity, gender, and age) and centrality (measured via network relationships) on stock market performance over a 15-year period. Using biographical data from the ISS Directors database and financial data from CRSP and COMPUSTAT, we built a dataset of 1500 firms. Through various network and regression analyses, we investigated if these leadership metrics can serve as predictors for outperformance against baseline market returns.

---

## Project Scope and Objectives

- **Primary Goal:**  
  Uncover correlations between board-level diversity/centrality metrics and firm performance.

- **Key Objectives:**
  - **Metric Definition & Data Collection:**  
    Quantify diversity and centrality measures. Combine financial data with biographical details to form a robust dataset.
  - **Analysis & Modeling:**  
    Use Python’s NetworkX to build leadership network graphs and run regression analyses (OLS models) to determine the statistical significance of these metrics.
  - **Insights:**  
    Evaluate whether understanding these metrics could potentially help outperform a baseline market return.

---

## Data Collection and Methodology

- **Data Sources:**
  - **Biographical Data:** ISS Directors database  
  - **Financial Data:** CRSP and COMPUSTAT

- **Key Metrics:**
  - **Diversity Metrics:**  
    Ethnicity (Herfindahl–Hirschman Index), Gender Diversity (% non-male), Age statistics (mean, range, entropy).
  - **Centrality Metrics:**  
    Betweenness, Closeness, Degree, and Eigenvector Centrality (computed using Python’s NetworkX).

- **Methodology:**
  - **Pipeline:**  
    Data collection, preprocessing, and augmentation to accurately define our metrics.
  - **Modeling:**  
    Running multiple OLS regression models, with and without control variables, to tease out statistically significant relationships.
  - **Visualization & Analysis:**  
    Correlation matrices and alpha plots to understand feature importance and potential redundancy in the network data.

---

## Key Findings

- **Centrality Insights:**  
  - Metrics like betweenness, eigenvector, and closeness centrality showed statistically significant correlations with firm performance.
  - For example, lower betweenness centrality (indicating a more tightly connected board) correlated with better stock returns.
  
- **Diversity Observations:**  
  - The impact of diversity metrics was mixed. While some trends hint at a relationship, the results indicate that more research is needed to fully understand the effects.
  
- **Model Performance:**  
  - Our control model achieved an R-squared of 0.029, while incorporating biographical metrics bumped it up slightly to 0.035. It’s not earth-shattering, but it certainly gives us some food for thought!

I personally find these results fascinating—especially how nuanced the effects of leadership structure can be on firm performance. It’s a reminder that sometimes, the devil really is in the details.

---


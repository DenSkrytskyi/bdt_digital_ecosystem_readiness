# BDT Digital Ecosystem Readiness - Mini Project

## Overview

This project provides a **data-driven snapshot of digital ecosystem readiness** using a carefully selected set of ITU indicators.  
The indicators cover five key dimensions: **Access, Usage, Infrastructure, Affordability, and Cybersecurity**.  

This analysis aligns with **ITU-D and BDT priorities**, demonstrating trends research, readiness assessment, and ecosystem thinking for digital transformation initiatives.

---

## Indicators Used

| # | Indicator | Dimension | Units |
|---|-----------|-----------|-------|
| 1 | Individuals using the Internet | Usage | % |
| 2 | Households with Internet access at home | Access | % |
| 3 | Population coverage, by mobile network technology | Infrastructure | % |
| 4 | Mobile broadband low-consumption basket (1 GB) | Affordability | % GNI per capita |
| 5 | Global Cybersecurity Index - Overall Score | Cybersecurity | Index |

> **Note:** Affordability is **inverted** during analysis: lower cost results in higher readiness.

---

## Project Structure

- **data/** - cleaned CSV files for each indicator  
- **notebook/** - analysis and visualizations (all charts embedded)  
- **figures/** - exported key visualizations ([click here to view](figures/))  

### Key Points for HR

- All visualizations are **embedded directly in the notebook**.  
- You can also **browse the exported charts directly in the `figures/` folder** on GitHub.  
- The composite index is calculated as the **average of normalized indicators** across the five dimensions.

---

## Analytical Approach

1. **Data Preparation**  
   - Latest available year per country  
   - Harmonized country codes (`entityIso`)  
   - Numeric-only values  

2. **Normalization**  
   - Min-Max scaling (0-1) for comparability  
   - Affordability inverted (lower cost = higher readiness)  

3. **Readiness Dimensions**

| Dimension | Indicator |
|-----------|-----------|
| Access | Households with Internet access at home |
| Usage | Individuals using the Internet |
| Infrastructure | Population coverage, by mobile network |
| Affordability | Mobile broadband low-consumption basket (1 GB) |
| Cybersecurity | Global Cybersecurity Index |

4. **Composite Readiness Score**  
   - Equal-weight average of normalized indicators  
   - Visualized as **bar charts** and **corr**

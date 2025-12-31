# BDT Digital Ecosystem Readiness – Mini Project

## Overview

This project provides a data-driven snapshot of digital ecosystem readiness using a **small, clean set of ITU indicators**. 
The selected indicators cover five key dimensions: Access, Usage, Infrastructure, Affordability, and Trust.  
This aligns with ITU-D and BDT priorities and demonstrates trends research, readiness assessment, and ecosystem thinking.

---

## Indicators Used

| # | Indicator | Dimension | Units |
|---|-----------|-----------|-------|
| 1 | Individuals using the Internet | Usage | % |
| 2 | Households with Internet access at home | Access | % |
| 3 | Population coverage, by mobile network technology | Infrastructure | % |
| 4 | Mobile broadband data and voice low-consumption basket (70 min, 50 SMS, 1 GB) | Affordability | % GNI per capita |
| 5 | Global Cybersecurity Index – Overall Score | Trust | Index |

---

## Project Structure

- **data/** – cleaned CSV files for each indicator  
- **notebook/** – analysis and visualizations (all charts embedded)  
- **figures/** – export of key visualizations  

### Key Point for HR

All analytical outputs and visualizations are **embedded in the notebook**.  
You can **open the notebook directly on GitHub** to review results without running any code.

---

## Analytical Approach

1. **Data Preparation**  
   - Latest available year  
   - Harmonized country codes (`entityIso`)  
   - Numeric-only values  

2. **Normalization**  
   - Min–Max scaling (0–1) across countries for comparability  
   - Affordability inverted (lower cost = higher readiness)  

3. **Readiness Dimensions**  

| Dimension | Indicator |
|-----------|-----------|
| Access | Households with Internet |
| Usage | Individuals using Internet |
| Infrastructure | Population coverage (mobile) |
| Affordability | Mobile broadband low-consumption basket |
| Trust | Global Cybersecurity Index |

4. **Composite Readiness Score**  
   - Equal-weight average of normalized indicators  
   - Visualized as radar charts, country ranking  

5. **Policy Insights**  
   - High access but low usage → skills / relevance gap  
   - Good infrastructure but poor affordability → pricing / competition issues  
   - High usage but low trust → cybersecurity capacity gap

---

## License

Data sourced from **ITU and Global Cybersecurity Index**.  
Project prepared for demonstration purposes aligned with **BDT Digital Ecosystem Roster** requirements.

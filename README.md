



## Project Overview

This project conducts an in-depth Exploratory Data Analysis (EDA) on the Titanic passenger data (`titanic.csv`) to investigate how **Family/Group Size** and **Group Type** influenced survival rates. The analysis specifically differentiates between true family members and non-family groups (e.g., friends, servants) traveling on the same ticket.

**Analysis Date:** June 19, 2025

## Key Findings and Conclusions

The analysis utilized two main approaches: **Case 1** (all passengers on a ticket are 'Family') and **Case 2** (passengers are classified as 'Family' or 'Non-Family' based on `FamilySize` vs. Ticket member count).

### Survival Driven by Family Cohesion and Gender

1.  **Small Families Excel:** Small families (2-4 members) in 1st class showed the highest survival rates (up to 0.8). Cohesion enhances survival compared to larger or non-family groups.
2.  **Female-Led Success:** Female-dominant families had survival rates of approximately 0.8, strongly supporting the 'women and children first' policy.
3.  **Family vs. Non-Family Advantage (Case 2):** Family groups (mean survival 0.45) significantly outperformed Non-Family groups (mean survival 0.30). The 162 Non-Family tickets likely represent friends or servants.
4.  **Large Groups Struggle:** Larger Non-Family groups, particularly those in 3rd class, showed the lowest survival rates (<0.2) due to logistical challenges.

### Socioeconomic and Statistical Factors

5.  **Class Disparity:** The best survival outcomes were consistently found among 1st-class small families, while 3rd-class large groups fared the worst.
6.  **High-Fare Advantage:** High-fare, small families in 1st class exhibited higher survival, reflecting the impact of wealth.
7.  **Correlation Insights (Heatmap):** Family Survival Rate showed a strong **negative correlation with Pclass** (-0.34) and a **positive correlation with FemaleCount** (Sex: 0.54).
8.  **Statistical Significance:** The Chi-square test for Case 2 confirmed that group size and type **significantly impact survival** (p-value: 0.0000).

### Passenger Distribution

*   **Total Passengers:** 891 (314 females, 577 males).
*   **Solo Travelers:** 547 of the 681 tickets were solo travelers.
*   **Class Distribution:** 3rd class was the largest, with 347 males and 144 females.

## Technical Details

| Component | Detail |
| :--- | :--- |
| **Dataset** | `titanic.csv` |
| **Libraries** | `pandas`, `numpy`, `matplotlib`, `seaborn`, `scipy.stats` |
| **Solo Travelers** | 547 tickets (FamilyMembers = 1) |
| **Inconsistent Fares** | 1 ticket found with varying fares |





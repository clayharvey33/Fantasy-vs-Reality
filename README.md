# Fantasy vs Reality  
### Quarterback Fantasy Scoring vs NFL Team Success

---

## Overview
This project analyzes whether fantasy football quarterback scoring is correlated with real NFL team success and evaluates alternative scoring systems to determine how closely fantasy performance aligns with actual winning outcomes.

The analysis uses team-season data from NFL seasons spanning 2016–2025 and compares multiple fantasy scoring formats against team win percentage.

---

## Key Question
Do fantasy football quarterback scoring systems reflect real NFL team success, and can they be improved to better align with winning outcomes?

---

## Data
- Source: Pro Football Reference  
- Time Period: 2016–2025 NFL seasons  
- Level of Analysis: Team-season  
- Target Variable: Team win percentage  
- Features: Aggregated quarterback passing and rushing statistics  

---

## Methodology
- Data was collected and cleaned from Pro Football Reference  
- Datasets were combined and standardized using SQL (SQLite)  
- Quarterback statistics were aggregated at the team-season level  
- Multiple fantasy scoring systems were constructed:
  - Standard scoring
  - Rushing Nerfed scoring
  - Passing Buffed scoring
  - Regression-informed scoring
  - Final proposed scoring system  
- Correlation analysis was used to measure relationships with team win percentage  
- Linear regression was used to evaluate the relative importance of quarterback performance variables  

---

## Key Findings
- Quarterback fantasy scoring is strongly correlated with NFL team success across all scoring systems (r ≈ 0.57–0.67)  
- Modified scoring systems show only slightly stronger correlations than standard fantasy scoring  
- Passing touchdowns and turnovers are more strongly associated with team success than yardage-based statistics  
- Rushing production appears less predictive of winning compared to passing efficiency and turnovers  
- Regression-based and final proposed scoring systems produced the strongest observed correlations, though improvements over standard scoring were modest  

---

## Visualizations
The analysis includes multiple visualizations comparing the relationship between fantasy scoring systems and NFL team success. These include correlation summaries and scatterplots across all evaluated scoring formats, all of which are displayed in the accompanying notebook.

---

## Limitations
- Analysis is conducted at the team-season level, limiting game-level detail  
- Correlation does not imply causation  
- Fantasy scoring is based on traditional box-score statistics and excludes advanced metrics such as EPA or QBR  
- Results are limited to NFL seasons from 2016–2025  

---

## Tools Used
- Python (Pandas, NumPy, SciPy, Statsmodels)  
- SQL (SQLite)  
- Jupyter Notebook  

---

## Conclusion
Fantasy football quarterback scoring systems show a consistent and statistically significant relationship with real NFL team success across all evaluated formats.

While differences between scoring systems are relatively small, modified and regression-informed scoring systems—including the final proposed system—generally produce slightly stronger correlations with team success than standard fantasy scoring.

These findings suggest that quarterback fantasy production is a stable indicator of NFL team success, and that fantasy scoring systems can be modestly adjusted to better reflect real-world performance without fundamentally changing the structure of the game.

# Election_AD_Spend

##  Objective
Analyze election-related advertising spend across Indian constituencies and election phases to uncover trends, outliers, campaign efficiency, and correlation with voter turnout and total votes.

---

##  Datasets Used
- `results.csv`: Voter data by parliamentary constituency (PC), phase, turnout, total votes.
- `advertisers.csv`: Facebook advertiser data with page name, ad spend, and disclaimer (sponsor).
- `locations.csv`: Location-level aggregate ad spend.

---

##  Key Analyses

###  1. Data Cleaning & Merging
- Standardized `PC_Name` across datasets.
- Converted ad spend to numeric and handled missing values.
- Merged voter and ad data based on constituency.

###  2. Correlation Analysis
- Heatmap revealed moderate positive correlation between ad spend and voter turnout.
- No strong correlation with total vote count.

###  3. State-Level Insights
- Horizontal bar chart used for clear comparison.

###  4. Phase-wise Efficiency
- Calculated `Ad Spend per Vote` metric.
- Phase 2 had the highest spend per vote; Phase 4 was the most efficient.
- Used dual-axis plot (bar + line) to compare efficiency and turnout.

###  5. Outlier Detection
- Applied Z-score to identify constituencies with anomalous ad spend.
- Flagged unusually high or low-spending regions for deeper inspection.

###  6. Party-wise Ad Spend
- Grouped ad spend by `Disclaimer` to estimate party-wise spend.
- Visualized top 10 political sponsors (e.g., BJP, INC, AAP).

---

##  Visualizations
-  Correlation heatmap
-  Horizontal bar charts (states, sponsors)
-  Phase-wise dual-axis chart (spend & turnout)
-  Scatterplot (spend vs turnout)
-  Outlier summary table

---

##  Key Insights
- High ad spend ≠ guaranteed high turnout.
- Ad saturation varies dramatically between regions.
- Campaign ROI (votes per rupee) fluctuates by phase.
- Outliers indicate possible over-investment or overlooked regions.

---

##  Tools & Technologies
- **Python**, **Pandas**, **Seaborn**, **Matplotlib**, **Scipy**
- Notebook format: **Google Colab** / **Jupyter Notebook**

---

##  Outcome
Delivered a reproducible analysis pipeline to evaluate electoral ad strategy performance across constituencies and phases — applicable for political consultants, media auditors, or policy think tanks.

---

# EPL Winner Predictor: A Data-Driven Analysis for the 2025–2026 Season  

## Project Overview  

This project analyzes the last three seasons of English Premier League (EPL) match data to identify patterns, evaluate performance factors, and predict the likely champion for the **2025–2026 season**. Using statistical tests and machine learning models, the analysis provides insights into team strengths, home vs. away advantages, and predictive indicators of success.  

---

## Project Objectives  

1. **Predict the 2025–2026 EPL Champion**  
   Build a model to forecast team wins and identify the most likely league winner.  

2. **Explore Match Performance Factors**  
   Evaluate how goals, shots, fouls, and cards influence match outcomes.  

3. **Assess Home vs. Away Advantage**  
   Statistically test differences in performance and scoring patterns between home and away games.  

4. **Identify Key Team Trends**  
   Highlight dominant clubs, emerging contenders, and relegation risks based on predicted win totals.  

---

## Data Source  

- **Dataset**: [Football-Data.co.uk](https://www.football-data.co.uk)  
- **Seasons**: 2022–23, 2023–24, 2024–25  
- **Records**: 1,140 matches, 133 attributes per match  
- **Scope**: Match metadata (goals, shots, fouls, cards, referees). Bookmaker odds excluded to prevent data leakage and improve future applicability.  

---

## Data Cleaning & Preparation  

- **Dropped Odds Columns**: Excluded bookmaker odds to avoid unrealistic prediction bias.  
- **Retained Core Match Metadata**: Goals, shots, fouls, corners, cards, referees.  
- **Datetime Transformation**: Converted date/time fields for proper sequencing and seasonal grouping.  
- **Standardization**: Stripped whitespace and ensured categorical consistency (e.g., referee names).  
- **Final Dataset**: Clean, structured match-level data ready for exploratory and inferential analysis.  

---

## Key Analyses & Insights  

### 1. Exploratory Data Analysis (EDA)  
- **Shot Distribution**: Majority of home teams take 10–18 shots; high-shot matches show skewness toward outliers.  
- **Goals**: Most games finish with 0–3 goals.  
- **Referees**: Anthony Taylor and Michael Oliver officiated the most matches.  

### 2. Inferential Analysis  
- **Home Advantage**:  
  - *T-tests and Wilcoxon tests* confirmed that home teams statistically take more shots and score more goals.  
- **Referee Effect**:  
  - ANOVA and Chi-Square tests show referees do **not** significantly influence goals or match outcomes.  
- **Correlation Tests**:  
  - Shots and goals show a weak but statistically significant positive correlation (r ≈ 0.23).  

### 3. Predictive Modeling  
- **Method**: Random Forest Regression  
- **Target**: Predicted total wins per team for the 2025–26 season  
- **Top Predictions**:  
  1. **Liverpool** – 22.7 wins  
  2. **Manchester City** – 22.2 wins  
  3. **Chelsea** – 20.3 wins  
  4. **Arsenal** – 20.0 wins  

---

## Tools & Technologies  

- **Python 3.11**  
- **Libraries**: Pandas, NumPy, Matplotlib, Seaborn, SciPy, Scikit-learn  
- **Notebook**: Jupyter for exploration and modeling  
- **Visualization**: Histograms, scatterplots, correlation matrices, and bar charts  

---

## Strategic Insights  

### 1. Title Contenders  
- Liverpool and Manchester City remain frontrunners, with Arsenal and Chelsea keeping pressure as consistent top-four challengers.  

### 2. Mid-Table Solidity  
- Newcastle, Brentford, Aston Villa, and Bournemouth project strong stability with 15–17 wins each.  

### 3. Poor Performers  
- Man United and WestHam.  

### 4. Future Model Enhancements  
- Incorporating **player-level statistics, injuries, squad depth, and financial factors** would refine predictions.  
- Real-time seasonal updates could allow **dynamic mid-season forecasting**.  

---

## Conclusion  

The **2025–26 EPL Winner Predictor** suggests that **Liverpool** are the most likely champions with **22.7 wins**, narrowly surpassing **Manchester City (22.2 wins)**. Chelsea and Arsenal round out the top four, confirming the continued dominance of historically strong clubs.  

While mid-table teams show resilience, and bottom-tier clubs face survival challenges, the model underscores the inherent unpredictability of football. Future improvements integrating richer player and financial data could sharpen accuracy. Nonetheless, this project establishes a **data-driven framework** for anticipating EPL outcomes, blending statistical rigor with sports analytics to guide fans, analysts, and stakeholders alike.  

---

## Contact  

**Author**: Brian Kiprop Kibor  
**Email**: kipropbrian26@gmail.com  
**Location**: Oulu, Finland  

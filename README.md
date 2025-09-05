# winnipeg-jets-analytics

## Project Overview
This project provides an in-depth analysis of the Winnipeg Jets’ performance in the NHL using advanced analytics techniques. It covers:

1. **Team-level analysis** – correlation heatmaps to understand team statistics and performance patterns.
2. **Player clustering** – KMeans clustering for skaters and goalies to identify performance groups and player roles.
3. **Stanley Cup prediction** – XGBoost model predicts the probability of the Winnipeg Jets winning the Stanley Cup.
4. **Weakness analysis** – compares Jets’ performance with the Top 10 NHL teams to identify gaps.
5. **Improvement recommendations** – suggests top players to strengthen weak positions and visualizes insights via radar charts.

This project demonstrates expertise in **Python, Pandas, Matplotlib, Seaborn, Scikit-learn, XGBoost**, and **data visualization**.

---

## Dataset
The project uses the following datasets:

- `Teams_clean.csv` – team-level statistics.
- `Skaters_clean.csv` – individual skater statistics.
- `Goalies_clean.csv` – individual goalie statistics.
- `Winners.csv` – past Stanley Cup winners for supervised modeling.

> ⚠️ If datasets are proprietary or large, include sample CSVs or instructions for obtaining them.

---

## Project Structure
NHL_Analytics_Project/
│
├─ Teams_clean.csv
├─ Skaters_clean.csv
├─ Goalies_clean.csv
├─ Winners.csv
├─ nhl_analytics.py # Team & player clustering analysis
├─ jets_stanleycup_predictor.py # XGBoost Stanley Cup prediction
├─ jets_weakness_analyzer.py # Identify team & player weaknesses
├─ jets_improvement.py # Recommend top players & radar visualization
├─ output/ # Generated CSVs and plots
└─ README.md


---

## Key Features

### 1. Team Correlation Heatmap
- Generates a heatmap to visualize correlations between team-level statistics.
- Identifies relationships between key performance indicators.
- Output: `output/team_correlation_heatmap.png`.

### 2. Player Clustering
- KMeans clustering for skaters and goalies.
- PCA 2D visualization for clusters.
- Helps identify player performance patterns and top-performing groups.
- Outputs: `output/skaters_clusters.csv`, `output/goalies_clusters.csv` and PCA plots.

### 3. Stanley Cup Prediction
- XGBoost classifier predicts the probability of winning the Stanley Cup.
- Uses team stats, top skaters, and best goalie stats.
- Example: *Winnipeg Jets: 35.7% probability of winning the Stanley Cup.*

### 4. Weakness Analysis
- Compares Jets’ team and player metrics against the Top 10 NHL teams.
- Identifies weaker areas such as GF/GP, PP%, Net PP%, Shots/GP, and FOW%.
- Analyzes goalies and skaters separately for actionable insights.

### 5. Improvement Recommendations
- Suggests top skaters to strengthen weak positions (C, L, R, D).
- Generates radar charts comparing Jets vs Top 10 average team metrics.
- Visualizes gaps in team and player performance for strategic decisions.

---

## Usage

```bash
# Team & player clustering analysis
python nhl_analytics.py

# Stanley Cup prediction
python jets_stanleycup_predictor.py

# Weakness analysis
python jets_weakness_analyzer.py

# Improvement recommendations & radar chart
python jets_improvement.py


# Premier-League-2023-2024-Prediction

This project is part of '"Introduction to DataScience Class" By analyzes football player data from the 2023/2024 Premier League season using descriptive and predictive data science techniques. It also explores the likelihood of player transfers based on performance and playtime.

## Objectives

- Analyze player statistics such as goals, assists, minutes played, age, and more.
- Identify "underused stars" — high-performing players with limited playtime.
- Predict which players may request transfers in the next season.
- Use regression models and cross-validation to estimate next-season performance.

## Contents

- `EPL Analyst.ipynb`: Main Jupyter Notebook containing the full analysis, feature engineering, and modeling.
- `premier-player-23-24.csv`: Dataset used (not pushed to GitHub due to size/privacy).
- Visuals: Age distribution, prediction results, feature importance, etc.

##  Key Features

###  Descriptive Analysis
- Age distribution of players
- Goals and assists per 90 minutes
- Positional averages (FW, MF, DF, GK)

###  Predictive Modeling
- Linear regression on expected goals (`xG`), assists (`xAG`), and progressive play metrics
- Cross-validation (`KFold`) for predicting future performance
- Custom scoring formula for **Transfer Opportunity Index**:
  - Based on `UnderusedStar`, `AgeScore`, and positional average

###  Transfer Prediction Logic

Players likely to request a move are identified based on:

- Above-average performance (goals/assists per 90 mins)
- Below-average match starts in their position
- Young age (higher `AgeScore`)

###  Example Output: </ba>

<img width="585" height="262" alt="Screenshot 2568-07-29 at 13 35 36" src="https://github.com/user-attachments/assets/f907add5-a6cb-40c5-98a1-8563a1329721" /> </ba>

<img width="1118" height="530" alt="Screenshot 2568-07-29 at 13 40 38" src="https://github.com/user-attachments/assets/40a621f6-ee43-4d77-a5b0-4f877b9ec884" />

<img width="1117" height="530" alt="Screenshot 2568-07-29 at 13 40 19" src="https://github.com/user-attachments/assets/04fb6bc0-8616-4b6e-85fb-db83116a423b" />

<img width="682" height="329" alt="Screenshot 2568-07-29 at 13 41 56" src="https://github.com/user-attachments/assets/642b61e6-034a-447d-b071-34560c687b20" />


## Tools 

- Python 3.12
- Jupyter Notebook
- Pandas, NumPy
- scikit-learn (LinearRegression, KFold)
- Matplotlib, Seaborn




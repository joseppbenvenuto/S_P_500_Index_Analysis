# S_P_500_Index_Analysis

## Project Description

In the below analysis, the S&P 500 Index closing prices will be explored within four decades. The objective is to analyze the index and determine if the index is an invaluable long term investment.

Four decades:

Decade 1: 1979 - 1989<br>
Decade 2: 1989 - 1999<br>
Decade 3: 1999 - 2009<br>
Decade 4: 2009 - 2019<br>

The analysis will seek to understand the compounded returns (not including dividends) the index has produced in the above time frames. 

Within each time frame, A/B will be performed to see if the means of prices between decades are statistically significant. The goal is to observe if the closing prices are higher or lower between the time frames and determine the risk of the investment. 

Further, Monte Carlo simulations will be performed to further asses risk. Using the Monte Carlo results, an average compounded return will be calculated to observe the simulated annual returns in addition to the actual compounded results in each time frame.

## Methods Used

1) Descriptive Statistics - used for preliminary data exploration.
2) Inferential Statistics - used to explore risk in the S&P 500 Index closing prices. 
3) Monte Carlo Simulations - used to explore risk in the S&P 500 Index closing prices.

## Results 

### A/B Tests and Monte Carlo Simulations

Time frame combinations:

Note - all p-values are significant at p < 0.05.

* **Decade 1 and Decade 2** -

* **Decade 1 and Decade 3** - 

* **Decade 1 and Decade 4** -

* **Decade 2 and Decade 3** - 

* **Decade 2 and Decade 4** - 

* **Decade 3 and Decade 4** - 

![](ReadMe_Images/Feature_Importance.png)

1) **Shooting Percentage** (shootingPctg)
2) **Save Percentage** (savePctg)
3) **Shots Per Gam**e (failedShotsPerGame)
4) **Percentage of Games Won when Team Scores First** (winScoreFirstGreater61_low)
5) **Save Per Game** (savesPerGame) 

Model Target:

1) **Above the Mean Adjusted Wins** (aboveMeanAdjWins)

Model results on test data:

![](ReadMe_Images/r2.png)

* **r2:** 0.90
* **Mean Absolute Error:** 1.79
* **Mean Squared Error:** 5.32
* **Root Mean Squared Error:** 2.31
 
### Logistic Regression Using Predicted Season Outcomes to Predict Playoff Outcomes

Model Feature:

1) **Predicted Above the Mean Adjusted Wins** (predAboveMeanAdjWins)

Model Target:

1) **Failed Seasons By Not Making Playoffs** (failed_playoff_flag)

![](ReadMe_Images/ROC_AUC.png)

* **Concordance:** 0.94
* **AUC:** 0.94

![](ReadMe_Images/CAP_LIFT.png)

* **Accuracy:** 0.86
* **Percision:** 0.91
* **Recall:** 0.87
* **F1:** 0.89
* **Kolmogorov–Smirnov Measure (KS):** 43% at the 4th decile, 1.1 time greater than a random model

### A/B Testing on Predictor Features

If teams want to make the playoffs they need to increase their aboveMeanAdjWins. To increase their aboveMeanAdjWins, teams should take into consideration the following:

Note - all A/B tests were significant as <0.05. 

1) **shootingPctg** -                strive to achieve **10.84%** shooting percentage and stay within range **10.3%, 10.48%, 10.67%**.<br>
2) **savePctg**                      strive to achieve a **90.21%** save percentage and stay within range **90.02%, 90.21%, 90.4%**.<br>
3) **savesPerGame**                  strive to achieve **26.12** saves per game and stay within range **25.82, 26.12, 26.42**.<br>
4) **failedShotsPerGame**            strive to achieve **27.17** shots per game and stay within range **26.91, 27.17, 27.43**.<br>
5) **winScoreFirstGreater61_low**    strive to win **82%** of games they score first and stay within range **75%, 82%, 88%**.<br>
6) **aboveMeanAdjWins**              strive to achieve **4.3** shots per game and stay within range **3.62, 4.3, 4.98**.<br>

## Technologies 

1) Python 
2) R
3) Jupyter Notebook
4) Anaconda Environment

## Order of Analysis

1) NHL_1983_2020_Multiple_Linear_Regression_EDA.ipynb
2) NHL_1983_2020_Multiple_Linear_Regression.ipynb
3) NHL_1983_2020_Logistic_Regression_EDA.ipynb
4) NHL_1983_2020_Logistic_Regression.ipynb
5) NHL_1983_2020_Feature_A-B_Tests.ipynb

## Directory Files

1) **NHL_API.ipynb** - NHL data base API.
2) **Preprocessing_Functions.ipynb** - Preprocessing functions.
3) **Regression_Metrics_Function.ipynb** - Rgression evaluation functions.
4) **AUC_CAP_Functions.ipynb** - Classification evaluation metrics.
5) **Stats_Functions.ipynb** - Descriptive and inferential stats functions.
6) **CHAID_Tree_Plots** - CHAID tree algorithm used to explore data for derived variables.
7) **NHL_1983_2020_Multiple_Linear_Regression_EDA.ipynb** - Multiple linear regression EDA, feature enginearing, and feature selection.
8) **NHL_1983_2020_Multiple_Linear_Regression.ipynb** - Multiple linear regression model building, feature selection, preprocessing, evaluation, and interpretation.
9) **NHL_Season_Wins_Linear_Regression_Model.pkl** - Saved multiple linear regression model.
10) **NHL_1983_2020_Logistic_Regression_EDA.ipynb** - Logistic regression EDA, feature enginearing, and feature selection.
11) **NHL_1983_2020_Logistic_Regression.ipynb** - Logistic regression model building, feature selection, preprocessing, evaluation, and interpretation.
12) **NHL_Playoffs_Logistic_Regression_Model.pkl** - Saved Logistic regression model.
13) **NHL_1983_2020_Feature_A-B_Tests.ipynb** - A/B testing on predictor features between successful and unsuccessful playoff outcomes.

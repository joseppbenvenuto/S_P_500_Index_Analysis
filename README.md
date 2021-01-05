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

**Note** - all p-values are significant at **p < 0.05**.

**Decade 1 and Decade 2** - 
* With 95% confidence, the difference in mean closing prices can be found between **-386.29 and -366.81**.
* The index returned simulated average compounded return of **6%** and at no time during the simulation had prices been lesser in decade 2 than in decade 1.
* If The investor bought the S&P 500 Index at the beginning of Decade 1 and sold at the end of Decade 2 (20 years), the investor would have earned an actual compounded return of **14%**.

**Decade 1 and Decade 3** - 
* With 95% confidence, the difference in mean closing prices can be found between **-1056.13 and -1041.1**.
* The index returned simulated average compounded return of **7%** and at no time during the simulation had prices been lesser in decade 3 than in decade 1.
* If The investor bought the S&P 500 Index at the beginning of Decade 1 and sold at the end of Decade 3 (30 years), the investor would have earned an actual compounded return of **8%**.

**Decade 1 and Decade 4** -
* With 95% confidence, the difference in mean closing prices can be found between **-1611.35 and -1566.89**.
* The index returned simulated average compounded return of **6%** and at no time during the simulation had prices been lesser in decade 4 than in decade 1.
* if The investor bought the S&P 500 Index at the beginning of Decade 1 and sold at the end of Decade 4 (40 years), the investor would have earned an actual compounded return of **8%**.

**Decade 2 and Decade 3** - 
* With 95% confidence, the difference in mean closing prices can be found between **-683.86 and -660.27**.
* The index returned simulated average compounded return of **4%** and at no time during the simulation had prices been lesser in decade 3 than in decade 2.
* if The investor bought the S&P 500 Index at the beginning of Decade 2 and sold at the end of Decade 3 (20 years), the investor would have earned an actual compounded return of **6%**.

**Decade 2 and Decade 4** - 
* With 95% confidence, the difference in mean closing prices can be found between **-1236.59 and -1188.55**.
* The index returned simulated average compounded return of **4%** and at no time during the simulation had prices been lesser in decade 4 than in decade 2.
* if The investor bought the S&P 500 Index at the beginning of Decade 2 and sold at the end of Decade 4 (30 years), the investor would have earned an actual compounded return of **8%**.

**Decade 3 and Decade 4** - 
* With 95% confidence, the difference in mean closing prices can be found between **-563.71 and -517.3**.
* The index returned simulated average compounded return of 2% and at no time during the simulation had prices been lesser in decade 2 than in decade 1.
* if The investor bought the S&P 500 Index at the beginning of Decade 3 and sold at the end of Decade 4 (10 years), the investor would have earned an actual compounded return of **4%.**

The S&P 500 Index has proven to be a profitable investment with a high margin of safety through a longer time horizon. <br>
Over the 40-year time frame, the actual annual compounded return for the index is 9%.<br>
A 100,000 investment at the beginning of the 40-year time frame would now be worth 3,140,942 today.<br>

**Note** - In addition, returns have been slowing down in the recent decade and can be explained by the unprecedented low interest rate environment.

## Technologies 

1) Python 
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

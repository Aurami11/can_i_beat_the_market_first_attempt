# can_i_beat_the_market_v1.0.0

## Overview

This project explores market trend prediction using both simple logic and machine learning techniques. The primary goal is to evaluate whether historical data can be used to predict stock movements within the complex financial market.

## Data Sources

- **Financial Data**: The model was tested using historical financial data, primarily from 2018 to 2019. Due to missing values, the dataset was reduced to approximately 200 days of data.
- **Additional Data Sources**: While other potential data sources were considered, technical limitations prevented their inclusion in this project.

## Approach & Methodology

Two key approaches were utilized:

1. **Supervised Machine Learning**: This approach employed machine learning models to predict stock prices. Although the R² value was generally low (and at times negative), this result is expected in financial modeling due to the inherent uncertainty in the market. Nonetheless, some predictions yielded surprisingly relevant insights.

2. **Theoretical Matrix-Based Approach**: This approach, inspired by theoretical frameworks, utilized matrix calculations to generate predictions. While more conceptual, this method provided valuable insights into the modeling process and offered an enriching learning experience.

### Models Used:
- **Linear Regression**
- **Gradient Boosting**
- **Decision Trees (Supervised Learning)**

## Results

Despite relatively low R² values and occasionally negative results, the predictions demonstrated intriguing potential. Below are the details from the Linear Regression model for APPL stock prices:
```
                                 OLS Regression Results                                
=======================================================================================
Dep. Variable:        PRICE_VARIATION   R-squared (uncentered):                   0.217
Model:                            OLS   Adj. R-squared (uncentered):              0.033
Method:                 Least Squares   F-statistic:                              1.179
Date:                Thu, 20 Mar 2025   Prob (F-statistic):                       0.244
Time:                        06:27:11   Log-Likelihood:                         -265.45
No. Observations:                 189   AIC:                                      602.9
Df Residuals:                     153   BIC:                                      719.6
Df Model:                          36                                                  
Covariance Type:            nonrobust                                                  
==============================================================================
                 coef    std err          t      P>|t|      [0.025      0.975]
------------------------------------------------------------------------------
Year           0.0004      0.000      2.308      0.022    5.09e-05       0.001
Month          0.0256      0.046      0.560      0.576      -0.065       0.116
Day           -0.0282      0.010     -2.917      0.004      -0.047      -0.009
Weekday       -0.1035      0.068     -1.529      0.128      -0.237       0.030
C_pca_1       -0.2846      0.575     -0.495      0.622      -1.422       0.852
C_pca_2       -0.6202      1.989     -0.312      0.756      -4.549       3.308
C_pca_3        0.6729      2.305      0.292      0.771      -3.881       5.227
C_pca_4       -3.1412      3.396     -0.925      0.356      -9.849       3.567
F_pca_1        0.8455      1.675      0.505      0.614      -2.463       4.154
F_pca_2       -4.9061      2.300     -2.133      0.035      -9.451      -0.361
F_pca_3        0.5686      2.364      0.241      0.810      -4.101       5.238
F_pca_4       -4.4942      3.075     -1.461      0.146     -10.570       1.581
F_pca_5        3.9198      3.343      1.172      0.243      -2.685      10.525
F_pca_6       -2.6428      3.359     -0.787      0.433      -9.279       3.994
F_pca_7       -4.2797      3.550     -1.206      0.230     -11.292       2.733
F_pca_8        1.9335      4.109      0.471      0.639      -6.185      10.052
F_pca_9        0.7982      4.250      0.188      0.851      -7.597       9.194
F_pca_10      -3.0737      4.334     -0.709      0.479     -11.635       5.487
F_pca_11      -3.1820      4.958     -0.642      0.522     -12.978       6.614
F_pca_12      -8.0271      4.923     -1.630      0.105     -17.754       1.700
F_pca_13     -10.1919      4.845     -2.104      0.037     -19.763      -0.621
F_pca_14      -3.2314      5.422     -0.596      0.552     -13.944       7.481
F_pca_15      -0.4922      5.140     -0.096      0.924     -10.647       9.662
F_pca_16      -4.9297      6.004     -0.821      0.413     -16.791       6.932
F_pca_17      -0.6426      6.118     -0.105      0.916     -12.730      11.445
F_pca_18      10.0559      6.208      1.620      0.107      -2.209      22.321
F_pca_19       3.8522      6.686      0.576      0.565      -9.356      17.061
F_pca_20       1.7716      6.573      0.270      0.788     -11.213      14.757
F_pca_21       3.4551      7.127      0.485      0.629     -10.624      17.535
F_pca_22       6.4796      7.188      0.901      0.369      -7.721      20.680
F_pca_23      -0.0933      7.440     -0.013      0.990     -14.791      14.605
T_pca_1       -3.3119      3.573     -0.927      0.355     -10.370       3.746
T_pca_2       -3.4994      4.451     -0.786      0.433     -12.293       5.294
T_pca_3       -8.0739      5.791     -1.394      0.165     -19.515       3.368
T_pca_4        1.2868      6.292      0.205      0.838     -11.143      13.717
T_pca_5       11.0996      6.934      1.601      0.112      -2.600      24.799
==============================================================================
Omnibus:                        7.834   Durbin-Watson:                   1.982
Prob(Omnibus):                  0.020   Jarque-Bera (JB):               13.961
Skew:                          -0.088   Prob(JB):                     0.000930
Kurtosis:                       4.320   Cond. No.                     2.14e+05
==============================================================================

Notes:
[1] R² is computed without centering (uncentered) since the model does not contain a constant.
[2] Standard Errors assume that the covariance matrix of the errors is correctly specified.
[3] The condition number is large, 2.14e+05. This might indicate that there are
strong multicollinearity or other numerical problems.

```

Although the results did not show strong predictive power, some variables and features still demonstrated potential for better understanding stock price variations.

## Progress & Next Steps

The next step involves extending the training dataset by increasing the time period from 2018-2019 to 2018-2022. This expansion will provide a broader range of data, allowing the model to learn from more diverse market conditions and potentially improve its predictive performance.

If successful, the model could later be used as a scenario generator for future market analyses once the project is complete.

## Conclusion

While the model's results are far from perfect, they indicate that machine learning techniques can be valuable tools for analyzing and predicting market trends, especially when working with historical data. Future improvements are essential to enhance the model's robustness and expand its application to longer periods of data.

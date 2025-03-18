# can_i_beat_the_market_v1.0.0

## Project Overview

This project explores market trend prediction using simple logic and machine learning techniques. The goal is to assess whether certain data can be used to anticipate stock movements, particularly in the complex financial context.

## Data Sources

- **Financial Data**: I used historical financial data to test the model, primarily from 2018-2019, although missing data reduced the dataset to about 200 days.
- **Other Sources**: Additional data sources were explored, but technical constraints limited their use in this project.

## Approaches and Methodology

Two main approaches were employed:

1. **Supervised learning with machine learning**: This method applied machine learning models to predict stock prices. The results showed a generally low R², and sometimes even negative, but this is understandable in the context of finance, where uncertainty is always present. Despite this, the predictions were surprisingly relevant in some cases.

2. **Theoretical approach based on matrix calculations**: A more conceptual approach was implemented, inspired by theoretical ideas. This also yielded interesting results, and the experience of its implementation was particularly enriching.

### Models Used:
- Linear Regression
- Gradient Boosting
- Supervised learning based on Decision Trees

## Results

Despite a low R² and sometimes negative results, the predictions showed interesting potential. This tool could have been useful as an indicator back in 2018. Below are some visual results from the tests conducted:


## Progress and Next Steps

I plan to test the model on more recent data. While I am not overly optimistic about improving the results, this will allow me to reduce the time interval between predictions and scale down to less than 1 day, providing more data for model training.

For privacy reasons, this project is intentionally vague. If I manage to achieve solid results, it could later serve as a scenario generator for future analyses once the project is completed.

## Note

I have carried out this project alone, from contextualization to the current application. However, I am considering seeking feedback from an expert for the next steps and potentially collaborating in the future.

## Conclusion

The project has shown that, while the results are not perfect, there is potential for applying these techniques to analyze and predict market trends, especially with historical data. Improvements are necessary to make the model more robust and extend it to longer periods of data.

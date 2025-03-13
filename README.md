# can_i_beat_the_market_v1.0.0

## Project Overview

This project is an attempt to predict market trends using simple logic and machine learning. The idea is to leverage global news data from GDELT and financial data from Yahoo Finance to build a predictive model. The goal is to understand whether news sentiment and financial market data can help forecast stock movements.

## Data Sources

- **GDELT**: I used the GDELT database to gather global news data. However, processing this data was quite challenging due to its large size and complexity. I was initially aiming to cover 10 years of data, but due to the data's weight and the need for extensive cleaning, I had to limit the scope to 3 years.
  
- **Yahoo Finance**: For the asset prices, I utilized the `yfinance` API to retrieve historical stock data. Unfortunately, due to data limitations, I could only retrieve daily prices rather than high-frequency data.

- **News Websites**: I attempted to scrape news websites for additional insights, but many of the sites were either inaccessible or difficult to scrape, limiting the data I could use.

## Tools & Technologies Used

- **OpenAI API**: I used various OpenAI models, including GPT-3.5, GPT-4 (mini), and MISTRALAI, to process the text data from GDELT. However, the size and complexity of the data caused issues in the second phase of the process (post-data cleaning and scraping).
  
- **Data Aggregation & Compression**: Given the large volume of data, I encountered challenges in aggregating and compressing the data in a way that makes it usable for model training.

## Challenges Faced

- **Data Processing**: The GDELT data was difficult to process due to its size and the complexity of handling news data at a global scale. This required significant preprocessing, and I had to reduce the timeframe of the data from 10 years to 3 years.
  
- **Data Access Issues**: Several news websites were either un-scrapable or blocked, preventing me from incorporating a wide range of news sources into the dataset.

- **Large Data Volumes**: The sheer volume of the data made it difficult to complete the second phase of processing. Data aggregation and compression techniques are still being worked on to handle this.

## Progress & Next Steps

- **Phase 1 Completed**: The first phase of the project, which involved scraping and processing the GDELT data, has been completed. 
- **Phase 2**: Currently, I’m working on finishing the second phase of data processing, which involves further aggregating and compressing the data to make it suitable for model training.
  
- **Model Training**: Despite having a dataset under 20,000 records, which should allow for relatively quick training, I still need to address the issues of data aggregation and compression before proceeding with model training.

## Conclusion

While progress is ongoing, there are still several challenges to overcome, especially around data processing and aggregation. However, the fact that my dataset is under 20,000 records should allow for faster training once the data issues are resolved. I am optimistic that once these hurdles are cleared, the project will be able to test the feasibility of using simple logic and news data to predict market trends.

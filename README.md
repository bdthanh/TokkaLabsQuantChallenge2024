# Tokka Labs Quant Challenge 2024

**Competition link**: [Tokka Labs Quant Challenge 2024](https://www.kaggle.com/competitions/tokka-labs-quant-challenge-2024/overview)

### Overview

In this competition, you need to showcase your machine learning skills in predicting short-term returns in the ever-changing crypto markets.

You will build a model that captures alpha signals and makes predictions against futures. Your final score is calculated over the next 10 days (01/03/2024 - 10/03/2024) using live data and promises valuable insights into financial forecasting amidst evolving market dynamics and transient signals.

### Evaluation 

Submissions are evaluated by Pearson correlation coefficient. We will calculate the score by averaging the correlation coefficient between your predicted return series and the real market return series of the 10 assets (AVAX, ADA, SOL, BNB, TRX, DOGE, LINK, XRP, BTC, ETH).

![Pearson correlation coefficient](images\image.png)

### Final results

- **Final Rank**: Secured a position within the top six on the leaderboard.
- **Correlation Coefficient**: Achieved an average Pearson correlation coefficient of 0.04705, indicating an acceptable positive relationship between the predicted and actual returns.
- **Prize**: Awarded a consolidation prize of USD 1,000 for my performance. 

![Final leaderboard](images\leaderboard.png)

### My approach

- **Model Development**: Utilizing the LightGBM (Light Gradient Boosting Machine) framework, I developed a predictive model that efficiently captures the complex dynamics of the financial markets. LightGBM was chosen for its high performance, scalability, and ability to handle large datasets with many features, making it ideal for financial time series analysis.

- **Integration of Open-Source Alphas**: A significant aspect of my methodology was the integration of open-source alphas — predefined trading signals based on historical price, volume, and fundamental data. By leveraging these open-source strategies, I enriched my model's feature set with proven indicators that enhance predictive accuracy. Implementing these alphas allowed me to incorporate a wide range of market sentiments and trading dynamics into my predictions.

- **Ensemble Strategy**: I experimented and decided implemented an ensemble of 24 distinct LightGBM models for each cryptocurrencies to further refine the predictive power. They were trained with different sets of features and data folds.
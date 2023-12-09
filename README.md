# research_sales_forecast_models
store related topics and resources

Croston model
Basic Croston
A first simple approach to predicting intermittent demand series is the Croston model, which takes a three step approach:
- evaluate the average demand level when there is a demand occurrence
- evaluate the average time between two demand occurrences
- forecast the demand as the demand level (when there is an occurrence) multiplied by the probability of having an occurrence.


- Croston model gets you through univariate cases with gaps and zeros.
- LGBM is the way to go for handling multiple series at once
- hybrid approach to predicting new products

Use of Embeddings: Kaggle: https://www.kaggle.com/code/konradb/ts-4-sales-and-demand-forecasting/notebook

Alternative approach:

- create embeddings for the categorical part with cat2vec https://openreview.net/pdf?id=HyNxRZ9xg
- cluster the products for which we know the sales
- calculate average target per cluster
- map the new ones to the nearest cluster

# Temporal Graph Convolutional Network for Predicting Ternary Stock Movement
The stock market is notoriously challenging to predict, prompting continuous advancements in forecasting models. One common forecasting task is stock movement prediction - predicting whether a stock price will increase or decrease. In this paper, we attempt to increase movement prediction accuracy via a novel ternary movement labeling scheme with separate labels for when a stock price significantly increases, significantly decreases, or remains relatively the same. This paper trains a Temporal Graph Convolutional Network (TGCN) architecture on five years of historical data from companies in the S\&P 500 and a larger superset of 2,415 stocks from the NYSE and NASDAQ Exchanges. Leveraging the temporal capabilities of the TGCN, the approach captures the temporal dependencies inherent in the stock market's complex network, as well as the relationships (edges) between stocks (vertices) both across and within sectors.

Our model performed best on the 2,415 stock superset, where the stocks we predicted to be positive outperformed the market average by 4x (for an overall daily increase of 0.60%). We also classified stocks as positive with a precision of 68% (although we sacrificed recall for this result, and classified nearly 95% of stock movements as unknown).

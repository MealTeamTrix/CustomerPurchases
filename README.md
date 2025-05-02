🛍️ Online Shopping Session Analysis

This project analyzes customer behavior in an online shopping dataset to understand purchasing patterns and statistical probabilities around sales performance. It includes customer segmentation, correlation analysis, and a binomial probability model to estimate sales outcomes.

📂 Dataset

File: data/online_shopping_session_data.csv

Each row represents a user session with features such as:

Page interaction counts and durations
Bounce and exit rates
Page values and special day impact
Customer type (New or Returning)
Whether a purchase was made (0 or 1)
Month and weekend session indicator
📊 Key Analysis Steps

1. Data Loading and Filtering
Load the dataset using pandas.
Focus the analysis on sessions in November and December.
2. Customer Segmentation
Compare session counts and purchase rates between New and Returning Customers.
Calculate:
Total sessions per group
Purchase rates for each group
3. Correlation Analysis
Use scipy.stats.pearsonr to find relationships between time spent on different page types.
Strongest correlation found between:
Administrative_Duration and Informational_Duration
4. Probability Modeling
Model the number of purchases among 500 sessions using a Binomial Distribution.
Simulate an improvement scenario with a 15% increase in purchase rate for returning customers.
Estimate the probability of making at least 100 sales using scipy.stats.binom.
5. Visualization
Plot the binomial probability distribution of potential sales from 500 sessions.
Highlight probability of reaching or exceeding 100 sales.
📈 Key Findings

New customers had a higher purchase rate (~27%) than returning customers (~19.6%).
With a 15% boost in the returning customer purchase rate:
There's ~90% probability of achieving at least 100 purchases in 500 sessions.

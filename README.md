# regression_days_prediction
anonymous sample, data science challenge to predict the number of order days in the month for each user

Context and goal:

- improve resource usage by predicting how many days in the month the user will spend in the month.
- (this prediction should be updated continuously throughout the month)

The goal of the exercise is to predict the number of order days for each user in August 2022, even when:

- Some order data is available for certain users,

- Or when no order data is available at all (users with NaN values).


The prediction is the remaining orders left for the month. If a user places 3 orders on the 10th,
20th, and 30th. We would want our predictions before the 10th to be 3, before the 20th to be 2, etc.

The already known orders in 'august_with_missing_order_days.parquet'.
The file ' historical_orders.parquet ' contains the users' historical transaction.
The file 'august_total_sales.parquet ' contains the forecasted total transaction amount in August
for each user. can treat it as the true value for the total monthly sales ( this information can help to make better predictions but is not a must )

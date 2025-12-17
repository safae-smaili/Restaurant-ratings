# Restaurant-ratings
**In this project, I used JSON datasets from the Yelp website that had more than 180,000 rows in total.**

**First, I started by exploring all 6 available tables and removed any duplicated tables (which I found - one was identical to another). Then, I merged them all into one table using the business_id.**

**I found myself with a huge table containing more than 180,000 rows and 36 columns. I began by studying the columns to understand what they contained, checking for any duplicated columns, and examining what useful information I could extract from the JSON-formatted columns. I discovered something really useful: the tables contained information not just for restaurants, but also for other types of businesses like salons and shops, so I removed those.**

**I continued the work and ended up with only numerical columns. I dealt with missing values—sometimes by removing them and sometimes by replacing them with the mean or 0, depending on the situation.**

**Then, I moved on to feature engineering, correlation analysis, creating new columns, and selecting the best ones for the model. Next, I split the data and scaled it because there was a huge difference between the values of the columns (even though the algorithm is linear regression and it doesn't depend on this scaling much) I fed the data into a linear regression model and achieved these results: R² = 0.66, RMSE = 0.6, MAE = 0.45.**

**Therefore, this model can predict with 0.6 accuracy the rating of a restaurant based primarily on review sentiment analysis, whether it's good for kids, review recency, and other features.**

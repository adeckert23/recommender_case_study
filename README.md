# Recommender Case Study

Building a movie recommendation system from the movielens dataset.

Tackled the cold start issue, by using KMeans clustering to cluster users based on age and sex as my initial model, as even just something that simple with this size data set, took some time to set up.  This was a very sparse data set, so to make predictions with so little information would have been tough.  So I clustered users, and then making predictions based on those clusters, helped me fill in the data set.  Then when I ran the Alternating Least Squared (ALS) model against the hidden data set, the score I ultimately got was higher, because the data I trained on was not as sparse.

I also ran a Grid Search to check which parameters would be most meaningful, and ultimately best.  This was how I fine tuned the model at the end.

03/18/2019 08:58:37 AM : DEBUG : score=4.27985347985348

Top 5% of our predicted movie ratings had an actual average rating of 4.28

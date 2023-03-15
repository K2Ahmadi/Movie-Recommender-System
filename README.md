# Movie-Recommender-System

Using PySpark on Azure databricks, I developed a movie recommendation system using ALS(Alternating Least Square) collaborative filtering approach.

The provided data (users and their movie ratings) is preprocessed and transformed into a user-item matrix using the ALS class from the pyspark.ml.recommendation module. The ALS class allows users to specify various hyperparameters such as the number of latent factors, the regularization parameter, and the number of iterations. Then, I train the model on the transformed data using the fit method, which returns an ALSModel object. This object can be used to generate predictions for user ratings on new movies using the recommendForAllUsers method. Finally, I evaluated the model using metrics such as root mean squared error (RMSE) to assess the model's performance. This helped me understand how well the model was performing and whether any further adjustments needed to be made.

After finalizing the model, I was able to generate the top 10 movie recommendations for several users. 

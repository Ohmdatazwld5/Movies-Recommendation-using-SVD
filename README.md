# Movies-Recommendation-using-SVD
//SVD - is a widely used technique for developing recommendation systems//

Singular Value Decomposition(SVD) - SVD is a classical method from linear algebra is getting popular in the field 
of data science and machine learning. This popularity is because of its application in developing recommender systems

   - A 'recommender system' is an intelligent system that predicts the rating and preferences of users on products
   
   - The primary application of recommender system is finding  a relationship between user and products in 
     order to maximise the user-product engagement
     
   - SVD is a 'matrix factorisation technique', which reduces the number of features of a dataset by reducing the space
     dimension from N-dimension to K-dimension (where K<N).In the context of the recommender system, the SVD is used as
     a 'collaborative filtering technique'.
     
   - Collaborative filtering technique uses a matrix structure where each row represents a user, and each column represent
     an item.
     
   - The elements of this matrix are the ratings that are given to items by users.
         ![image](https://user-images.githubusercontent.com/130119515/231925539-f2f1c7b5-25ea-4f79-8967-da259b2a1484.png)
         
   - Applying SVD: After creating the dataset object, the SVD algorithm is instantiated using the SVD() constructor.
   
   - The cross_validate() method of the surprise library is then used to compute the RootMean Squared Error (RMSE) and
     Mean Absolute Error (MAE) of the SVD algorithm. The cross_Validate() method performs cross-validation on the data using
     the specified number of folds (cv=3) and prints the RMSE and MAE values for each fold
     
     ![image](https://user-images.githubusercontent.com/130119515/231927279-57cbf004-a953-4bbb-af12-a37f3abf5965.png)
     
   - The above output shows the evaluation results of the SVD algorithm on the Netflix Price dataset using 3-fold cross-validation
     The RMSE and MAE values are computed for each fold and the mean and standard deviation are also calculated
     
   - Overall, SVD algorithm has achieved a reasonably "good performance" on the Netflix Prize dataset with a 
     mean RMSE of 0.9977 and a mean of MAE of 0.8029
     
   - Find all the movies that have been rated 5 stars by user with ID 712664 and displays the names of the movies
   ![image](https://user-images.githubusercontent.com/130119515/231929705-03727e7d-6b11-43f4-80ca-b29ee9f06985.png)

   
   - The above code predicts the ratings for user 712664 using the trained SVD model and creates a new column 
     'Estimated_Score' with the predicted ratings for each movie
     
   - The 'Movie_Id' column is then dropped from the dataframe, and the dataframe is sorted based on the predicted ratings in descending order. 
     The top 10 recommendations are printed using the head() method
   
   - Overall, the code recommends the top 10 movies for user 712664 based on their predicted ratings using the SVD algorithm



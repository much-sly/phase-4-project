# MOVIE RECOMMENDATION SYSTEM.

## NAME: SYLVIA MUCHIRI.

##  Business Understanding.

### SPECIFYING THE DATA ANALYTICS QUESTION.

Movies are a great way to pass time especially after a long day of work and all you can think about is something to help you relax. What if there was a recommender system that recommends movies based on ratings and how users. The recommender system makes recommendations based on previous movies you have watched and how you rated them so that you can be able to continue enjoying movies of your choice without much effort of looking.

###  PROBLEM STATEMENT.

In today's digital age, the entertainment industry is experiencing rapid growth, with an ever-expanding library of movies and TV shows available to audiences. However, this abundance of content often leads to decision fatigue among viewers who are overwhelmed by the choices. To address this issue and enhance the user experience, our objective is to make a movie recommendation system that will address this issue and reduce dissatisfaction when looking for a movie.

### MAIN OBJECTIVE.

The primary goal of this project is to develop a movie recommendation system that can provide personalized movie suggestions to users based on their preferences, viewing history, and behavior.

###  SPECIFIC OBJECTIVES

. To build a recommender system using user-user similarity.

. To find the optimal parameters to use for singular value decomposition.

. To use evaluation metrics such as the Root Mean Squared Error (RMSE) and the Mean Absolute Error (MAE) to check the performance of the model.

###  EXPERIMENTAL DESIGN.

. Data Collection

. Read and check the data

. Preprocessing the data

. Building the recommendation system.

. Conclusions and Recommendations

###  DATA UNDERSTANDING.

The dataset used in this project is from:
. Movielens dataset from the GroupLens research lab at the University of Minnesota. The dataset was specifically the "small" dataset containing 100,000 user ratings.

. It contains 100836 ratings and 3683 tag applications across 9742 movies. These data were created by 610 users between March 29, 1996 and September 24, 2018. This dataset was generated on September 26, 2018.

. Ratings are made on a 5-star scale, with half-star increments (0.5 stars - 5.0 stars). Only movies with at least one rating or tag are included in the dataset.

. Tags are user-generated metadata about movies. Each tag is typically a single word or short phrase. The meaning, value, and purpose of a particular tag is determined by each user.

### BUILDING THE RECOMMENDATION SYSTEM.
The recommendation system was built based on singular value decomposition(SVD) having hypertuned the parameters to find the optimal parameters. Thereafter, it was fit to the training data and finally made predictions is movie recommendations to a new user. This was done through building a function that prompts the user to make ratings for a movie. Through these ratings, the system is able to make recommendations to a user based on user- similarity. The evaluation metrics used to check the performance of the system was Root Mean Squared Error(RMSE) and Mean Squared Error(MAE). The system performed well and was able to provide recommendations for the new user.

### CONCLUSIONS.

. Effectiveness of collaborative filtering method, In this project I used user-user similarity which proved to be the right approach to take since there were fewer users than items. However there consists other methods like content based filtering are good approaches which can be customized to suit user preferences. 

. I used the singular value decompositions and generated a grid search in pursuit of the best parameters in order to make right predictions and cross validated using the KNNBasic and the KNNBaseline, the latter yielded better results in reducing the test rmse after making predictions. The optimum parameters were, n_factors = 20, n_epochs = 20, lr_all = 0.05, reg_all = 0.4 respectively.

. Implementing user friendly interfaces increases the chance of users rating a movie thus makes collection of metadata easier in order to provide insightful recommendations suited to the liking of the user.

. When working with a large dataset it is important to have adequate memory or use a sample of the data that is representative of the whole to make predictions, however using the entire dataset would yield better results since it is training and learning from a huge datset which makes it easier to make accurate predictions, consequently it is important to be cautious not to overfit.

### RECOMMENDATIONS.

. To address the cold start problem, that is, the system finds it difficult to make recommendations for users or items that have fewer interactions with it. Content-based methods and hybrid recommendation systems can address this issue by incorporating item features and metadata. 

. The performance of recommendation system depends on hyperparameter settings. Careful tuning of hyperparameters, such as the number of neighbors (k) in KNN or the regularization term in matrix factorization, is essential for optimal results. This can be done by using a grid search that takes in a range of values for different parameters and find the best parameters based on the problem at hand.

. To determine the recommendation system's performance it is important to use evaluation metrics, common metrics include Root Mean Squared Error (RMSE), Mean Absolute Error (MAE), F1 score among others. These metrics help you to guage how the system is performing and how to improve its prformance if it is low.

. The user experience should be a priority. Implement user-friendly interfaces that allow users to provide feedback, rate items, and refine their preferences. User feedback can be used to continuously improve recommendations.

. Ensure that the recommendation system has good security, this ensures trust between users and the system is built where they are guaranteed their information is kept safe, private or even anonymized.

. Hybrid recommendation systems are a great way to improve the performance of the system. These systems incorporate collaborative filtering, content-based filtering, and other techniques, however hese types require adequate memory in order to be able to run well.

. The recommendation system should be flexible in that they can correctly make recommendations even with changes either from the user's preferences or even accomodating new users.


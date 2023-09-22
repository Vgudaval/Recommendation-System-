
# Recommendation-System-

Hybrid Recommendation System

The method described is a machine learning model that predicts a numerical value (rating) based on model based recommendation system on a set of input features. Here are the steps in more detail:

Define the input features: The model uses a set of user and business features, including user_id, review_count, average_stars, useful, fans, yelping_since, cool, and funny for the user, and business_id, stars, latitude, longitude, review_count, is_open, attributes.BusinessAcceptsCreditCards, attributes.BikeParking, attributes.GoodForKids, attributes.HasTV, attributes.OutdoorSeating, attributes.RestaurantsReservations, attributes.RestaurantsTakeOut, attributes.RestaurantsGoodForGroups, attributes.RestaurantsDelivery, and attributes.OutdoorSeating for the business. Additionally, the number of photos per business, number of tips per business, and number of tips per user are also used as input features.

Train an XGBoost regressor: XGBoost is a machine learning algorithm that is commonly used for regression problems. The model is trained on a dataset of examples where each example contains the input features and the corresponding numerical rating.

Tune hyperparameters: The hyperparameters of the XGBoost algorithm are tuned to optimize the performance of the model.

Error distribution analysis: The model's performance is evaluated by analyzing the distribution of prediction errors. In this case, the errors are binned into ranges of ratings (e.g., >=0 and <1, >=1 and <2, etc.) and the number of examples in each bin is counted.

Calculate root mean squared error (RMSE): The RMSE is a commonly used metric to evaluate the performance of regression models. It measures the average distance between the predicted ratings and the true ratings in the dataset.

Overall, the described method is a machine learning model that predicts a numerical rating based on a set of input features which uses model based recommendation sysytem. The XGBoost algorithm is used with hyperparameters tuned to optimize performance, and the model's performance is evaluated using the error distribution and RMSE.

Error Distribution:

>=0 and <1: 102319

>=1 and <2: 32818

>=2 and <3: 6093

>=3 and <4: 812

>=4: 2

RMSE:
0.9775680229066512

Execution Time:
434.044s


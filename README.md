# cognifyz
Restaurant Data Analysis Project
Overview
This project involves analyzing a restaurant dataset and developing machine learning models for prediction and classification, as well as building a recommendation system. The project is divided into four tasks, each focusing on different aspects of restaurant data analysis, including prediction of ratings, recommendation systems, cuisine classification, and geographical analysis.

Task 1: Predicting Restaurant Ratings
Objective
The goal of Task 1 is to build a machine learning model that predicts the aggregate rating of a restaurant based on other features, such as price range, cuisine type, and location.

Steps
Preprocessing:
Handle missing values.
Encode categorical variables.
Split the data into training and testing sets.
Model Selection:
A RandomForestRegressor was chosen for predicting the ratings.
Model Training:
The model is trained using the training set.
Model Evaluation:
The model’s performance is evaluated using Mean Squared Error (MSE) and R-squared.
Libraries Used
scikit-learn for preprocessing, model training, and evaluation.
pandas for data manipulation.
Output
The model’s performance is assessed by printing the MSE and R-squared scores.

Task 2: Restaurant Recommendation System
Objective
Task 2 involves creating a content-based recommendation system that suggests restaurants to users based on their preferences, such as cuisine type and price range.

Steps
Preprocessing:
Handle missing values and encode categorical variables.
Criteria for Recommendations:
Users can specify preferences based on cuisine type, price range, and aggregate rating.
Content-Based Filtering:
Compute a cosine similarity matrix using the specified features.
Recommend restaurants that are most similar to the user's preferences.
Testing:
Provide sample user preferences and output recommended restaurants.
Libraries Used
scikit-learn for cosine similarity computation.
pandas for data manipulation.
Output
The system outputs a list of recommended restaurants based on user preferences.

Task 3: Cuisine Classification
Objective
Task 3 involves developing a machine learning model that classifies restaurants based on their cuisine type, using various features such as restaurant location, price range, and aggregate rating.

Steps
Preprocessing:
Handle missing values.
Encode categorical variables.
Split the dataset into training and testing sets.
Model Selection:
A RandomForestClassifier is chosen for classifying restaurants into different cuisine types.
Model Training:
Train the classifier on the training data.
Model Evaluation:
The model’s performance is evaluated using accuracy, precision, and recall.
Libraries Used
scikit-learn for classification and model evaluation.
pandas for data manipulation.
Output
The model's performance metrics (accuracy, precision, recall) are printed. The model also classifies restaurants into specific cuisine types.

Task 4: Geographical Analysis and Restaurant Visualization
Objective
Task 4 involves performing a geographical analysis of the restaurant dataset and visualizing restaurant locations on an interactive map. Additionally, the task includes aggregating key restaurant metrics (e.g., ratings and price ranges) by city or locality.

Steps
Geographical Visualization:
Calculate the average latitude and longitude to center the map.
Add markers for each restaurant with details (restaurant name and rating).
Create an interactive map using the folium library.
Data Grouping:
Group restaurants by City and calculate the following:
Average aggregate rating.
Average price range.
Number of restaurants per city.
Output:
Save the map as an HTML file.
Print a table summarizing the aggregated data by city.
Libraries Used
folium for interactive map creation.
pandas for data manipulation.
Output
An interactive restaurant map (saved as restaurant_map.html).
A table displaying aggregated metrics (average ratings, price ranges, and restaurant count) by city.

## IPL Score Prediction Project

### Introduction
In this project, I developed a machine learning model to predict the final score of an Indian Premier League (IPL) cricket match based on various features such as batting team, bowling team, overs played, runs scored, wickets taken, runs scored in the last 5 overs, and wickets taken in the last 5 overs.

### Data Collection
I gathered the dataset for this project from Kaggle, a popular platform for data science and machine learning. The dataset contains historical IPL match data, including information about teams, players, overs, runs, and wickets.

### Data Preprocessing
Before building the prediction model, I performed several preprocessing steps on the dataset to clean and prepare it for analysis. The steps include:
1. Importing necessary libraries such as pandas and numpy.
2. Loading the dataset into a pandas DataFrame.
3. Describing the shape and columns of the dataset.
4. Removing unwanted columns that are not relevant to score prediction.
5. Keeping only consistent teams that have participated in multiple IPL seasons.
6. Removing the first 5 overs data from every match to focus on predicting the final score.
7. Converting the 'date' column from string to a datetime object.
8. Encoding categorical features using one-hot encoding.
9. Splitting the data into training and testing sets.

### Model Building and Evaluation
I used four regression models to predict the final score:
1. Linear Regression
2. Decision Tree Regression
3. Random Forest Regression
4. AdaBoost Regression

For each model, I performed the following steps:
1. Created an instance of the model.
2. Fit the model on the training data.
3. Predicted the scores for the test data.
4. Evaluated the model's performance using metrics such as Mean Absolute Error (MAE), Mean Squared Error (MSE), and Root Mean Squared Error (RMSE).
5. Calculated the model's test score.

### Model Comparison and Selection
To compare the performance of the different models, I calculated the MAE, MSE, and RMSE for each model and visualized them using bar plots. Additionally, I calculated the accuracy of each model and plotted it on a bar plot. The model with the highest accuracy was selected as the final model.

### Score Prediction
Using the selected model, I implemented a function to predict the final score based on user inputs. The function takes inputs such as batting team, bowling team, overs played, runs scored, wickets taken, runs scored in the last 5 overs, and wickets taken in the last 5 overs. It returns a range of predicted scores.

### Web Application
I developed a Flask web application to provide a user interface for score prediction. The application consists of multiple HTML templates for the home page, result page, and report page. It also includes routes for handling user requests and rendering the appropriate templates. The trained model is loaded using pickle and used to predict scores based on user inputs.

### Conclusion
This IPL score prediction project demonstrates the application of machine learning techniques to predict the final score of cricket matches. By analyzing historical data and training regression models, it is possible to estimate the total runs scored in an IPL match. The developed web application provides an easy-to-use interface for users to obtain score predictions based on their inputs.

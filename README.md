# Titanic Survival Prediction Using Machine Learning

The sinking of the RMS Titanic in 1912 remains one of the most infamous maritime disasters in history,
leading to significant loss of life. Over 1,500 passengers and crew perished that fateful night. 
Understanding the factors that contributed to survival can provide valuable insights into safety protocols and social dynamics during crises. 
In this project, we will leverage machine learning techniques to predict the survival chances of Titanic passengers based on various features, 
such as sex, age, and passenger class. Using the Random Forest classification algorithm, 
we aim to build a predictive model that will allow us to estimate the likelihood of survival for each individual aboard the Titanic.

### Part A: Objective of the Project: Predicting Titanic Passenger Survival

The primary objective of this project is to develop a machine learning model capable of predicting the survival status of Titanic passengers based on available data. The dataset includes information such as demographic attributes (age, sex), socioeconomic status (fare, class), and other relevant features. By analyzing these features, we seek to identify patterns that could influence survival rates and subsequently use these insights to make predictions on unseen data.

There will be three main steps in this experiment:

- Feature Engineering
- Imputation
- Training and Prediction

For this project, we will utilize the Titanic dataset. The dataset consists of the following files:

1. train.csv: Contains information about the passengers and their survival status, which will be used for training our model. Serves as our primary data source for training and validation, providing both features and target labels.
2. test.csv: Includes details of passengers without survival labels, which we will use for making predictions. Allows us to assess the model's performance on unseen data, simulating a real-world scenario where predictions must be made for new passengers.
3. gender_submission.csv: A sample submission file that demonstrates the format required for submitting predictions.

### Part B: Step-by-Step Implementation: Predicting Titanic Survival
1. Importing Libraries and Initial setup
2. Data Visualization: Understanding Survival Trends and Passenger Demographics
3. Feature Engineering: Optimizing Data for Model Training
4. Model Training: Building the Predictive Model (with this, we got an accuracy of 86.59%)

In this phase, we employ Random Forest as our algorithm to train the model for predicting survival. Key steps include:

- Data Splitting: Dividing the dataset into 80% training and 20% testing subsets using train_test_split() from the sklearn library.
- Model Selection: Leveraging the Random Forest algorithm, known for its robustness and ability to handle diverse data.
- Performance Evaluation: Assessing the trained model's accuracy on the test data to ensure it generalizes well.

### Part C: Prediction: Generating Survival Predictions on Test Data

In this final phase, we use the trained Random Forest model to make predictions on the test dataset. The key steps are:

- Running Predictions: Input the test dataset into the trained model to predict survival outcomes.
- Preparing Results: Store the PassengerId from the test data and the corresponding Survival predictions (0 or 1).
- Saving the Output: Export the predictions to a CSV file for submission, with two columns:
    - PassengerId: ID of each passenger from the test dataset.
    - Survival: Predicted survival status (0 = Did not survive, 1 = Survived).

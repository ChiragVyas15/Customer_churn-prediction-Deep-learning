# Customer_churn-prediction-Deep-learning

This project is designed to predict whether a bank customer will churn (leave the bank) or not. It uses a dataset of customer information to build a machine learning model that can identify customers who are at a high risk of leaving.

Here is a step-by-step summary of the project's flow:

1. Data Loading and Understanding 📊
The project starts by loading the 
Churn_Modelling.csv dataset into a pandas DataFrame.
This dataset contains information about bank customers, including their credit score, age, gender, account balance, and whether they have "Exited" (churned) or not.

2. Data Preprocessing and Cleaning 🧼
Before the model can be trained, the data needs to be prepared. This involves several steps:
Dropping irrelevant columns: Features that are not useful for prediction, such as RowNumber, CustomerId, and Surname, are removed.
Encoding categorical data: The model can only work with numbers, so text-based columns like Geography and Gender are converted into numerical format using one-hot encoding.
Splitting the data: The dataset is divided into a training set (to build the model) and a test set (to evaluate its performance).

3. Building the Artificial Neural Network (ANN) 🧠
The core of this project is a deep learning model called an Artificial Neural Network (ANN).
The ANN is built using the Keras library and consists of:
An input layer that receives the customer data.
Two hidden layers that learn complex patterns from the data.
An output layer that produces the final prediction (a probability of whether the customer will churn).

4. Training the Model 🏋️‍♀️
The ANN is trained using the training data.
During training, the model is "compiled" with an optimizer (adam) and a loss function (binary_crossentropy), which help it learn effectively.
The model is trained over many "epochs" (iterations) to improve its accuracy.

5. Making Predictions and Evaluating Performance 📈
Once the model is trained, it is used to make predictions on the unseen test data.
The performance of the model is evaluated using two key metrics:

Confusion Matrix: This shows how many predictions were correct and how many were incorrect, giving a detailed view of its performance.

Accuracy Score: This provides a single number representing the percentage of correct predictions.

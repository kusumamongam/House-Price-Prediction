# House Price Prediction Using Machine Learning

## Project Overview

This project focuses on predicting house prices using Machine Learning and Linear Regression. It uses the Boston Housing Dataset to understand the relationship between different housing and neighborhood features and their corresponding house prices.

The project covers the complete machine learning workflow, including data exploration, preprocessing, feature scaling, model training, evaluation, and deployment through a Flask web application.

Users can enter the required housing attributes through a web interface and receive a predicted house price.

## Objectives

- Analyze housing data to understand the factors influencing house prices.
- Perform exploratory data analysis (EDA).
- Prepare and preprocess data for machine learning.
- Build a Linear Regression model for price prediction.
- Evaluate model performance using Mean Squared Error and R² Score.
- Deploy the trained model using Flask.

## Dataset Information

**Dataset:** Boston Housing Dataset

The dataset contains 506 observations and 13 input features.

The features used for prediction include:

- CRIM – Per capita crime rate
- ZN – Residential land zoning proportion
- INDUS – Non-retail business acres proportion
- CHAS – Charles River proximity indicator
- NOX – Nitric oxide concentration
- RM – Average number of rooms
- AGE – Proportion of older owner-occupied properties
- DIS – Distance to employment centers
- RAD – Accessibility to radial highways
- TAX – Property tax rate
- PTRATIO – Pupil-teacher ratio
- B – Dataset-specific demographic variable
- LSTAT – Percentage of lower-status population

**Target Variable:** MEDV (Median value of owner-occupied homes).

## Technologies & Libraries

- Python
- NumPy
- Pandas
- Matplotlib
- Scikit-learn
- Flask
- HTML

## Project Workflow

1. **Data Loading:** Load the Boston Housing Dataset using Scikit-learn.
2. **Exploratory Data Analysis:** Explore the dataset, understand feature distributions, and analyze correlations.
3. **Data Preprocessing:** Separate independent and dependent variables.
4. **Train-Test Split:** Divide the dataset into 70% training data and 30% testing data.
5. **Feature Scaling:** Apply StandardScaler to standardize input features.
6. **Model Building:** Train a Linear Regression model using the training dataset.
7. **Model Evaluation:** Evaluate predictions using Mean Squared Error and R² Score.
8. **Model Deployment:** Save the trained model and scaler using Pickle and integrate them into a Flask application.

## Model Performance

The notebook reports the following evaluation results:

| Evaluation Metric | Result |
|---|---:|
| Mean Squared Error (MSE) | 19.83 |
| R² Score | 0.7836 |

The R² score indicates that the model explains approximately 78.36% of the variance in the test dataset.

## Web Application

The project includes a Flask-based web application.

**Application workflow:**

1. Open the web application.
2. Enter the 13 required housing features.
3. Click the Predict button.
4. View the predicted house price.

The application loads the saved regression model and scaler to process user inputs and generate predictions.

## Project Structure

```text
House-Price-Prediction/
│
├── Regression.ipynb       # Model development and analysis
├── app.py                 # Flask application
├── templates/
│   └── home.html          # Web application interface
├── regmodel.pkl           # Saved regression model
├── scaler.pkl             # Saved feature scaler
└── requirements.txt       # Project dependencies
```

## Installation and Execution

**1. Clone the repository**

```bash
git clone https://github.com/kusumamongam/House-Price-Prediction.git
```

**2. Navigate to the project directory**

```bash
cd House-Price-Prediction
```

**3. Install the required libraries**

```bash
pip install -r requirements.txt
```

**4. Run the Flask application**

```bash
python app.py
```

**5. Open the application**

Visit the following address in your browser:

```text
http://127.0.0.1:5000/
```

Enter the required input values and click Predict to generate a house price prediction.

## Key Learning Outcomes

- Understanding regression problems in Machine Learning.
- Performing exploratory data analysis.
- Understanding independent and dependent variables.
- Implementing Linear Regression using Scikit-learn.
- Applying feature scaling using StandardScaler.
- Evaluating regression models using MSE and R² Score.
- Saving and loading machine learning models using Pickle.
- Deploying a machine learning model using Flask.

## Future Improvements

- Experiment with additional regression algorithms.
- Perform feature selection and model optimization.
- Improve the web interface and input validation.
- Deploy the application on a cloud platform.
- Explore more recent and representative housing datasets.

## Author

**Kusuma Mongam**

[GitHub Profile](https://github.com/kusumamongam)

---

*This project was developed for learning and demonstrating an end-to-end machine learning workflow, from model development to web application deployment.*

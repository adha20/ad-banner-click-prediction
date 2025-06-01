# Ad Banner Click Prediction using Logistic Regression

As part of the final mini project from the **"Machine Learning with Python for Beginner"** module at DQLab, I built a simple yet practical logistic regression model to predict whether a user will click on a promotional banner ad while browsing a website.

This project represents the culmination of everything I’ve learned throughout the course including data preprocessing, exploratory data analysis (EDA), model building using supervised learning algorithms, and model evaluation. I was able to apply those concepts to a real-world scenario using a structured dataset.

A bit of background: I worked on a dataset that includes user behavior features such as daily internet usage, time spent on site, age, and income. The goal was to classify whether or not a user would click on an ad. In doing so, I practiced data wrangling, data manipulation, data visualization, and performance evaluation using tools like confusion matrix and classification report.

Prior to this project, I completed all previous DQLab modules that covered the foundations of machine learning, both supervised and unsupervised, along with hands-on implementation using Python and scikit-learn.

---

## What's in this project...

The project follows a structured workflow consisting of:

1. Exploratory Data Analysis (EDA) 
2. Data preprocessing
3. Machine Learning - Ad Banner Click prediction with Logistic Regression
4. Evaluating the model using confusion matrix and classification report

---

## Dataset Overview

The dataset includes the following key features:

1. **Daily Time Spent on Site**: The amount of time (in minutes) the user spends on the site daily.  
2. **Age**: The user's age (in years).  
3. **Area Income**: The average income in the user's local area.
4. **Daily Internet Usage**: The average amount of time (in minutes) the user spends on the internet per day.  
5. **Ad Topic Line**: The topic/content of the promotional banner.  
6. **City**: The city from which the user accessed the website.  
7. **Male**: Indicates whether the user is male (1 = Male, 0 = Not male).  
8. **Country**: The country from which the user accessed the website.  
9. **Timestamp**: The time when the user either clicked on the promotional banner or left the website without clicking.
10. **Clicked on Ad**: Indicates whether the user clicked on the promotional banner (0 = No, 1 = Yes).

---

## Project Results

1. **Data Wrangling & Preprocessing**: I started by loading and inspecting the dataset. Fortunately, the dataset was clean there were no missing values. I removed some irrelevant columns such as `Ad Topic Line`, `City`, and `Timestamp` to keep only the numeric and relevant features. This step helped simplify the dataset for modeling. I also checked the datatypes to ensure everything was ready for the machine learning pipeline.

2. **Exploratory Data Analysis (EDA)**:  
   I visualized the distributions of features like `Daily Time Spent on Site`, `Daily Internet Usage`, and `Age` using Seaborn. The EDA revealed some interesting insights—for example, users who spent more time on the site tended to click on ads more often, while users with higher daily internet usage were less likely to click. A correlation heatmap showed that `Age` and `Daily Internet Usage` were important features related to the target variable.

3. **Modeling & Evaluation**:  
   I used **Logistic Regression** to build a classification model to predict whether a user would click the ad. The dataset was split into training and test sets with a 70:30 ratio. After fitting the model, I evaluated it using a confusion matrix, classification report, and ROC-AUC score. The model achieved strong performance with high precision, recall, and an AUC score that indicates it distinguishes well between classes.

   Overall, the model performed quite well, and the process helped me better understand the full machine learning workflow—from cleaning data to drawing insights and evaluating predictions.

---

##  Potential Improvements

- Test other classification models: Random Forest, SVM, or XGBoost  
- Implement hyperparameter tuning with `GridSearchCV` or `RandomizedSearchCV`  
- Extract additional features from the `Timestamp` column (e.g., hour, day)  
- Apply cross-validation for more robust performance estimates  
- Build a cleaner pipeline using `sklearn.pipeline` for maintainability and reproducibility  

---

##  Resources Used

- Krish Naik's YouTube tutorials  
- Machine learning courses on Udemy  
- Online articles from Stack Overflow, GeeksforGeeks, and Kaggle discussions  
- **ChatGPT** – for code troubleshooting, explanation of logistic regression concepts, evaluation techniques, and documentation support  

---

> Thank you for checking out this project! 🙌

# Ad Banner Click Prediction using Logistic Regression

As part of the final mini project from the **"Machine Learning with Python for Beginner"** module at DQLab, I built a simple yet practical logistic regression model to predict whether a user will click on a promotional banner ad while browsing a website.

This project represents the culmination of everything I’ve learned throughout the course including data preprocessing, exploratory data analysis (EDA), model building using supervised learning algorithms, and model evaluation. I was able to apply those concepts to a real-world scenario using a structured dataset.

A bit of background: I worked on a dataset that includes user behavior features such as daily internet usage, time spent on site, age, and income. The goal was to classify whether or not a user would click on an ad. In doing so, I practiced data wrangling, data manipulation, data visualization, and performance evaluation using tools like confusion matrix and classification report.

Prior to this project, I completed all previous DQLab modules that covered the foundations of machine learning, both supervised and unsupervised, along with hands-on implementation using Python and scikit-learn.



## What's in this project...

The project follows a structured workflow consisting of:

1. Exploratory Data Analysis (EDA) 
2. Data preprocessing
3. Machine Learning - Ad Banner Click prediction with Logistic Regression
4. Evaluating the model using confusion matrix and classification report



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



## Result of this project...

1. **Exploratory Data Analysis**: After loading the dataset, I began by examining the correlation matrix to identify relationships between features and the target variable. This analysis revealed that features such as Age, Daily Time Spent on Site, and Daily Internet Usage had significant correlations with the likelihood of clicking on an advertisement. Subsequently, I visualized the distributions of these key numerical features to understand their spread and detect potential outliers. Finally, I utilized a pairplot to explore the relationships between all features, providing deeper insights into how they might influence a user's likelihood to click on an advertisement.

2. **Preprocessing** I verified that the dataset contained no missing values or duplicate entries. Irrelevant columns were removed to simplify the modeling process. I also examined the features for outliers and applied feature scaling to ensure the numerical values were on similar scales, which is important for the performance of the logistic regression model.

3. **Modeling & Evaluation**: A Logistic Regression model was trained to classify whether a user would click on a banner ad or not. The dataset was split into training and testing sets using an 80:20 ratio. Model performance was evaluated using a confusion matrix and classification report.
   
   The evaluation results show that the model achieved an accuracy of 94% on the test data. It also demonstrated strong performance metrics across both classes, with a precision of 0.90 and recall of 0.97 for class 0 (not clicked), and precision of 0.97 and recall of 0.91 for class 1 (clicked). These metrics indicate a solid balance between sensitivity and specificity.
   
   Overall, the model performed quite well in predicting user behavior, generalizing effectively to unseen data. This end-to-end process from cleaning and analyzing the data to building and validating the model provided a comprehensive understanding of the machine learning workflow.


##  Potential Improvements

1. Try other classification algorithms such as Random Forest, SVM, or XGBoost to compare their performance with logistic regression.
2. Interactive visuals 
3. Extract additional features from the `Timestamp` column (e.g., hour, day).
4. Apply cross-validation for more robust performance estimates.
5. implement more complex python syntax (for example; use functions to simplify the codes).
   



##  Resources Used

1. Indonesia Belajar's YouTube  
2. Machine learning courses on DQlab 
3. Online articles from github and Kaggle 
4. ChatGPT: I use ChatGPT to evaluate code effectiveness, validate the analyses performed, assist in identifying more informative and appropriate data visualizations, etc.


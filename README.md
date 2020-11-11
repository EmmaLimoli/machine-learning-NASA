# machine-learning-challenge
use machine learning to process raw data

#The Goal: The goal for this project was to take the data from NASA Kepler space telescope from the past nine years and use Machine Learning to discover hidden planets outside of the solar system. 

#How This Was Achieved: The NASA Keopler space telescope data is from a planet-hunting mission from the past nine years. In the project, preprocessing the dataset was the first step, followed by tuning model parameters. Lastly, I chose two models to try and compare the outcomes to see the benefits of both options. The two models that I chose were Logisitc Regression and Random Forest.  

DISCUSS BEFORE pre-processing

#Model One: Logisitc Regression
For the first model, I chose Logisitic Regression since it's a classification algorithm. Since we're trying to figure out whether the are hidden planets outside of the solar system, that's a binary question.

The first step was pre-processing the data is using StandardScaler and LabelEncoder to scale the data. I created StandardScalers to fit X for train and test. The label encoder helps fit the y_train. Additionally, encoded helps to transform Y test and train. 

Then I imported LogisitcRegression model and fit the data to the scaled X train and the encoded Y train. Once that was complete, I created predictions and printed out the training and testing data score. The training data score is: 0.8867 and the testing 0.8947. 

I also imported classification reports to break down the planets that are confirmed, false positive, and candidate. This helps determine the chances of discovering hidden planets. 

Lastly, I used the GridSearch model for hyperparameter tuning. For the gird parameters I used 10, 50, and 100 for C and 200, 500, and 1000 for max_iter. Then I used grid fit for the X and Y train. The best params is 10, the best max_iter is 1000, and the best score is 0.6633.

In conslusion 

used StandardScaler and LabelEncoder

#Model Two: Random Forest
used MinMax Scaler

Tools Used: Python, sklearn, Pandas, Matplotlib, NumPy, train test split, MinMaxScaler, StandardScaler, LabelEncoder, Logistic Regression, Random Forest, Classification Report, GridSearch, JobLib 



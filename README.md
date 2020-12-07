<h1>Machine Learning Project</h1>
Use machine learning to process raw data
<br></br>
<strong>The Goal:</strong> 
<br></br>
The goal for this project was to take the data from NASA Kepler space telescope from the past nine years and use Machine Learning models to discover hidden planets outside of the solar system. 
<br></br>
<strong>How This Was Achieved:</strong> 
<br></br>
The NASA Kepler space telescope data is from a planet-hunting mission from the past nine years. In the project, preprocessing the dataset was the first step, followed by tuning model parameters to find out the possibility of additional planets being outside the solar system. I chose two models to try and compare the outcomes. The two models were Logisitc Regression and Random Forest.  

<h3>Model One: Logistic Regression</h3>
For the first model, I chose Logisitic Regression since it's a classification model. Since we're trying to figure out whether there are hidden planets outside of the solar system, that's a binary question.

The first step was pre-processing the data. I used StandardScaler and LabelEncoder to scale the data. I created StandardScalers to fit X for train and test. LabelEncoder helps fit the y_train. Additionally, LabelEncoder helps to transform Y test and train to make it easier to digest for the Logistic Regression model. 

I imported the Logistic Regression model and fit the data to the scaled X train and the encoded Y train. Once that was complete, I created predictions and printed out the training and testing data score. The training data score is: 0.8867 and the testing 0.8947. 

I also imported classification reports to break down the planets that are confirmed, false positive, and candidate. This helps determine the chances of discovering hidden planets. 

Lastly, I used the GridSearch model for hyperparameter tuning. For the gird parameters, I used 10, 50, and 100 for C and 200, 500, and 1000 for max_iter. Then I used grid fit for the X and Y train. The best param is 10, the best max_iter is 1000, and the best score is 0.6633.

In conslusion, the training and testing data were right 88% and 89% respectively. When studying the precision, recall, f1 score, and support breakdown, I found that the percentages were above 60%, which is what I was hoping for. 


<h3>Model Two: Random Forest</h3>
For the second model, I chose Random Forest because it's a classification model. The Random Forest model helps to build the different scenarios of the data based on the samples. This model will produce a prediction that's based on the average of the findings. Since we want to find out about hidden planets, this model will give us the average prediction of each outcome. 

Like the Logistic Regression model, I chose the features to run through the model. I deviate from the previous model at pre-processing since I used MinMaxScaler instead of Standard Scaler and LabelEncoder. I used MinMaxScaler because it would be beneficial to see the lowest and highest numbers of the sample set to better understand the average outcomes.

I imported RandomForestClassifer and fit it to the model. The training data was 1.0 and the testing data score was 0.88. I also printed the sorted zip of the selected features to better understand each other breakdowns for the features.

Lastly, like the Logisitic Regression model, I used GridSearch to narrow down and tune the results for the decision tree. For the param grid, I used 250, 300, and 350. Max depth I used 125, 150, and 175. The best score was 0.89. As for the precision, recall, f1-score, and support, the numbers like with Logisitic Regression were high. 

In conslusion, the training and test data were right 100% and 88% respectively. When studying the breakdown of precision, the precentages were above 60%, which again is what I was hoping for.  

<strong>Tools Used: Python, sklearn, Pandas, Matplotlib, NumPy, train test split, MinMaxScaler, StandardScaler, LabelEncoder, Logistic Regression, Random Forest, Classification Report, GridSearch, JobLib</strong> 



# Movie_Correlation_Analysis

<img width="962" alt="movie" src="https://user-images.githubusercontent.com/102785000/185897236-7dcc2430-eb42-4187-820c-b8c18eb838c4.png">

Nowadays, people are deeply influenced by the film industry from both financial and cultural aspects. What makes a movie successful from the financial perspective? Its gross earning has to be greater than its budget. But what's the correlation between the movie's gross revenue and its other features like genre, company, star, director, votes, etc? For investors, they don't want to put a great budget in something that has just a very small impact to the movie's earning. Therefore predicting movie features correlation is beneficial to our movie investors. 

Technologies:
Tableau, Python or Jupyter Notebook

Dataset: 


# Table of Contents

• Summary

• Visualization

• Python

• Correlation (Pearson)

• SMOTE

• Models(4) Traing, Testing, Prediction

• Conclusion

## Summary

This summary summarizes the steps of getting the prediction on the movie features by training and testing with four different machine learning models: RandomForestClassifier, AdaBoostClassifer, GradientBoostingClassifer, and ExtraTreeClassifier. The first step was to clean the dataset and assign variables for features and targets. The second step was to use Pearson Correlation to measure the strength of relationship between features. The third step was to balance the data with SMOTE technique. The last tep was to train and test the features in 4 different machine learning models to see which one has the highest accuracy. 

## Visualization

Used Tableau to visualize the film industry's overall growth on gross revenue from 1980 to 2020 and compare the different genre of movies vs it's revenue.

<img width="693" alt="tableau_png" src="https://user-images.githubusercontent.com/102785000/185898142-acff8df4-9b71-4c72-80cf-10c205793cf4.png">

## Python
Data Cleanining- dropped NAs and duplicates and converted data types.

<img width="391" alt="python1" src="https://user-images.githubusercontent.com/102785000/185994121-736d3769-724e-4214-bd5b-efc36dd19ddd.png">

<img width="423" alt="python2" src="https://user-images.githubusercontent.com/102785000/185994151-925f09f0-734a-4c57-bf4a-d9b5709a7327.png">

<img width="460" alt="python3" src="https://user-images.githubusercontent.com/102785000/185994227-8443397f-f47f-4d1a-be83-1d33f940522d.png">


<img width="415" alt="python4" src="https://user-images.githubusercontent.com/102785000/185994250-a3d39b75-d1a2-47ba-a956-e39de0689af8.png">


## Pearson Correlation

Correlation Matrix Heatmap showed high correlations between budget and gross earnings. 

<img width="937" alt="correlation" src="https://user-images.githubusercontent.com/102785000/185976499-8f933c62-8a13-41ea-a57b-0f9dd0b04acb.png">

## SMOTE
SMOTE technique was used to resample the imbalanced data. 

/Users/MiaHuang/Desktop/Movie_Correlation_Project/resample.png

## Machine Learning Models
• RandomForestClassifier

<img width="696" alt="randomforest" src="https://user-images.githubusercontent.com/102785000/185896981-89d5c39d-f3f9-40aa-9a08-aefef200f7bc.png">


• Ada Boost

<img width="648" alt="adaboost" src="https://user-images.githubusercontent.com/102785000/185896833-220fe274-bff7-4d9d-9031-0937d4bdbb09.png">

• GradientBoostingClassifer

<img width="651" alt="gradientBoosting" src="https://user-images.githubusercontent.com/102785000/185897045-35925ba5-8675-4346-aa6e-fa04d112dda1.png">


• ExtraTreesClassifier

<img width="630" alt="extratree" src="https://user-images.githubusercontent.com/102785000/185897572-f1c88300-a57c-4357-8311-80196f4e4872.png">

## Conclusion
In conclusion, for predict the success of a movie (gross revenue higher than budget), Gradient Boosting Classifer had the highest scores of accuracy, precision, recall, F1. 

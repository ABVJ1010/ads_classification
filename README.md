Author:

# Aidan Ben-Josef


We are tasked to create a model that would predict if a specific customer would purchase an add or not, based on a set of features they have. 
We have been working with 400 data points that    


[Notebook](https://github.com/ABVJ1010/ads_classification/blob/main/Aidan_Ben_Josef_Project_Advertisement_classifier.ipynb))


**Data dictionary** 
Data dictionary for [advertisments.csv]([./advertisments.csv]):


				
|Feature|Type|Description|
|---|---|---|
|**User ID**|*int64*|ID of the Person|
|**Gender**|*object*|Male or Female|
|**Age**|*int64*|age of the person|
|**EstimatedSalary**|*int64*|Estimated Salary |
|**Purchased**|*int64*|if the person bought the advertisment or not|

## Executive Summary

1. Import the libraries to make our code
2. Import the data that we acquired from kaggle
3. Check datatypes of features
4. Discarded User ID since it has no impact on the regression or prediction
5. The gender column is One Hot Encoded the Gender column due to it having categorical data in string form
6. Instantiate and fit a logistic regression to get AUC(0.7375415282392026)
7. Use Standard Scaler to scale the features
8. Instantiate and fit a new logistic regression to get new AUC(0.933856840833585)

## Conclusion

The AUC on the original data was ok but the scaled data is over 90%, so the scaled data produced a logistic regression on it.

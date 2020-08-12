## Project Name

How much you worth?


## Objecitve

The objective of this project is to provide salary estimate of professionals given a job description usign Machine Learning.



## Background 

For professional seeking to estimate their salary based on job title, location, Year of Expereince, Major in degree, Type of degree.



## The Predictive Task

Given the data, we can predict the salary of the job.

For this task I plan to use the mean square error (mse). Using error metric like precision and recall do not make sense as I am not predicting binary values or predicting classes. I predict an absolute value and the best way to find the error is by finding how much I missed the actual value by.

I am using the baseline model as linear regression predicting the salaries for all jobs. Here I am considering this as the baseline because this is a model which would give the estimate of mse. Anything below this is a useless model and probably the combination of features used should not be experimented further. Based on the knowledge of jobs and salary provided I focused my model on three features. First, years of experience; second, the location of the job; third, the category of the job; fourth


## Methodology

Throughout the jupyter notebook, I describe the process of connecting two datasets, cleaning data and finding useful features. For the prediction task, I tried several different supervised regression models, including Elastic Net, Lasso Regression, XGBoost Regressor, etc. I also use grid search to tune the parameters of different types of models, so thus to best fit the train data. After modeling, I checked with mse, feature importance to choose the optimal model. As a result, We are able to achieve a very accurate regressor by XGBoost Regressor. I built a pipeline that automates training model on entire training set, saves model to disk and scores the test dataset.

## Results

Based on the results it seems to be like that the Years of experience, Location and the Type of job help determine the salary. However, the degree or major does not effect the distribution of the salary.

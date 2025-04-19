### Analysis of Factors for Predicting Diabetes in Adult Populations

**Gabriel Diaz de Leon**

#### Executive summary

#### Rationale
In the United States, diabetes is prevalent in more than 10% of the population across all ages, while more than 20% of afflicted adults are unaware of their diagnosis. This means that the ability of a large portion of adults to gauge their own risk factors is poor, which could be improved by identifying which factors can be used as secondary indicators for adults to seek medical attention. Further, understanding the relationship between self-report measures and diagnostic outcomes can inform and improve doctors’ interactions with future patients. Earlier detection of diabetes is highly correlated with reduced medical costs, suggesting that improved diagnostic practices could alleviate a significant amount of burden on the healthcare system.

#### Research Goal
To identify the factors most closely related to, and investigate the efficacy of self-report measures in, determining a diabetes diagnosis

#### Data Sources
CDC Diabetes Health Indicators (UCI Machine Learning Repository)
https://archive.ics.uci.edu/dataset/891/cdc+diabetes+health+indicators

#### Methodology
•	Data Analysis
        - Correlation
•	Regression
        - Linear Regression
        - Logistic Regression
        - Lasso Regression/Regularization
        - Ridge Regression/Regularization
        - Feature Engineering (e.g. Lasso regression)
•	Classification
        - Logistic Regression
        - KNN
        - Decision Trees
        - Support-Vector Machine (SVM)
•   Feature Engineering (e.g. kernels for non-linear features)

#### Results
##### Expected Results:
•	Patient history is highly correlated with diabetes diagnosis
•	Greater socioeconomic capabilities negatively correlate with diabetes diagnosis (e.g. lower chance of diabetes)
•	Self-report measures have a high degree of correlation between each other
•	Few self-report measures are essential in classifying diabetes diagnoses

##### Preliminary Results:
###### Data cleaning:
        - Simple steps are taken to decode numerical category variables into values that represent the categorical groups (since not all classes are linearly distributed, this could change the classifier's performance)
        - The first education class is eliminated due to an extremely small amount of samples
        - Feature engineering is the final project goal, so the process of evaluating the influence of individual factors is excluded from the initial report
        - As a result, although there are many classes that are unbalanced across all factors, elimination of a factor will be tested thoroughly in the coming steps, and we have included all factors in the intial testing phases that follow
        - The 3-target dataset has an absurdly small amount of samples for the pre-diabetic class, which also decreases the samples for the diabetic class. As a result, we will focus on the 2-target dataset
###### Evaluation
        - Mean accuracy score is the main evaluation metric that will be used
        - As a reflection of a model's overall "correctness", this metric is useful since we have a clear target variable
        - 3 baseline models are used for comparison purposes: dummy model, health model, and body model
        - The separate baseline models allow us to get an initial idea of the influence that certain factors have on the efficacy of the classification models
        - The unbalanced target class could pose an issue when separating training and testing datasets, so we will test two different splitting methods
###### Conclusions
        - The different splitting methods lead to comparable results
        - The dataset is massive, evidenced by the enormous difference in processing times
        - The support vector machine is the classifier with the best results, with the greatest consistency between training and testing data sets, and also with an overwhelmingly large processing time.

#### Next steps
What suggestions do you have for next steps?

#### Outline of project

- Preliminary Results Notebook: (https://github.com/GabrielDiazdeleon/Berkeley_Capstone_Analysis-of-Factors-for-Predicting-Diabetes-in-Adult-Populations/blob/0e1e74cc0b96ae297abdfda51567c535a2eaaaf1/capstone_diabetes_preliminary.ipynb)


##### Contact and Further Information




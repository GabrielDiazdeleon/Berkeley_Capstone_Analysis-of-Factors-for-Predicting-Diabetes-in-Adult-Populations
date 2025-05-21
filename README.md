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
• Data Analysis
        - Data Exploration
        - Correlation
• Classification
        - Logistic Regression
        - KNN
        - Decision Trees
        - Support-Vector Machine (SVM)
        - Feature Engineering (e.g. kernels for non-linear features)
• Ensemble Techniques
        - Voting
        - Stacking
        - Boosting
        - Further feature engineering

#### Results
Expected Results:
•	Patient history is highly correlated with diabetes diagnosis
•	Greater socioeconomic capabilities negatively correlate with diabetes diagnosis (e.g. lower chance of diabetes)
•	Self-report measures have a high degree of correlation between each other
•	Few self-report measures are essential in classifying diabetes diagnoses

Preliminary Results:
•   Data cleaning:
        - The first education class is eliminated due to an extremely small amount of samples  
        - The 3-target dataset has an absurdly small amount of samples for the pre-diabetic class, which also decreases the samples for the diabetic class. As a result, we will focus on the 2-target dataset  
•   Evaluation  
        - F1 score is the primary evalutation metric due to the imbalanced target classes  
        - Accuracy is used as the algorithmic evaluation function for avoiding conclusion redundancies and overfitting  
        - 3 baseline models are used for comparison purposes: dummy model, health model, and body model  
        - The separate baseline models allow us to get an initial idea of the influence that certain factors have on the efficacy of the classification models  

Final Results:  
•   Evaluation  
        - All 3 baseline models are incapable of effectively classifying the dataset.  
        - While the performance of individual classification models have varying strengths and weaknesses, the logistic regression classifier performs best in terms of success rate and consistency.  
        - Boosting ensemble models performed well, although the stacking classifier was the optimum performing ensemble technique.  
        - Of all combinations tested, the stacking classifier performed best when limited to the feature pruning defined by the individual classification models.  
        - Further feature pruning exacerbates inconsistencies between performance for training and testing sets for ensemble techniques.  
•   Conclusions  
        - Individual health factors can inform a diabetes diagnosis in different ways.  
        - While no individual factor can be definitely taken out of consideration, certain base factors were identified.  
        - A patient's BMI, Age, general health report and whether they reported having high blood pressure or high cholesterol were the most influential factors regardless of model or technique.  
        - If patients are experiencing negative symptoms, especially those who have greater BMIs and are older, they should check with their doctor about whether diabetes is playing a role in their daily lives.  

#### Next steps
- Individuals with blood pressure and cholesterol issues should seek medical attention regarding diabetes on regular intervals  
- Since increased age and a BMI farther outside of the healthy range are significant indicators of potential diagnoses, these populations should also be mindful of their elevated risk  
- In future studies, the information included in self-report health metrics should be expanded to further understand how other patients can better monitor themselves  

#### Outline of project

- Preliminary Results Notebook: (https://github.com/GabrielDiazdeleon/Berkeley_Capstone_Analysis-of-Factors-for-Predicting-Diabetes-in-Adult-Populations/blob/0e1e74cc0b96ae297abdfda51567c535a2eaaaf1/capstone_diabetes_preliminary.ipynb)
- Final Results Notebook: (https://github.com/GabrielDiazdeleon/Berkeley_Capstone_Analysis-of-Factors-for-Predicting-Diabetes-in-Adult-Populations/blob/04ec464f49226f72fc3a315a3de5b2ea8a01d87b/capstone_diabetes_final.ipynb)


##### Contact and Further Information
Gabriel Diaz de Leon
diazdeleon.gabriel@gmail.com
+1 (773) 480-4639




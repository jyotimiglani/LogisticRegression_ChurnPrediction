# Telecom Churn Case Study

With 21 predictor variables we need to predict whether a particular customer will switch to another telecom provider or not. In telecom terminology, this is referred to as churning and not churning, respectively.

# Python Libraries Used

Pandas

Numpy

Scikit-Learn

Matplotlib

# Steps Involved:

1. Data Exploration

2. Data Cleaning

3. Feature Engineering

4. Feature Standardisation

5. Feauture Selection
  
    Correlation: Measures the degree to which two variables are related. Eliminated variables with high correlation
 
    RFE: Recursive feature elimination builds a model on the full set of features, and similar to the method above 
         selects a subset of features that are deemed most important by the model. 
         However, usually only a single feature is dropped from the dataset, and a new model is built with the 
         remaining features. 
         The process of dropping features and model building is repeated until there are only a pre-specified 
         number of features left. Selected 13 features.
  
    VIF: The Variance Inflation Factor (VIF) is a measure of colinearity among predictor variables within a 
         multiple regression. Eliminated variables with high VIF.

6. Model Building: Logistic Regression

7. Model Evaluation 

    Confusion Matrix: shows for each true class, how frequent a given predicted outcome is. 
                      You can read in detail about confusion matrix and terms associated with it 
                      https://medium.com/thalus-ai/performance-metrics-for-classification-problems-in-machine-learning-part-i-b085d432082b
                      
    ROC Curve: Receiver operating characteristics. A roc-curve works with uncertainty outputs of a classifier, 
                say the "cut off probability" for classification. Instead of making a cut-off at zero and 
                looking at classification outcomes, it looks at every possible cut-off and records how many 
                true positive predictions there are, and how many false positive predictions there are.

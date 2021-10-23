# Credit Risk Analysis. Project 17 of the UofT.
## `-Contents-`	
	
- [Overview of the Credit Risk Analysis](#Overview-of-the-Credit-Risk-Analysis)	
- [Resources](#resources)	
- [The Credit Risk Analysis Result](#The-Credit-Risk-Analysis-Result)
  - [Resampling Models to Predict Credit Risk ](#--Resampling-Models-to-Predict-Credit-Risk )
  - [The SMOTEENN algorithm to Predict Credit Risk](#--The-SMOTEENN-algorithm-to-Predict-Credit-Risk)
  - [Ensemble Classifiers to Predict Credit Risk](#--Ensemble-Classifiers-to-Predict-Credit-Risk)
- [The Credit Risk Analysis Summary](#The-Credit-Risk-Analysis-Summary)
## `Overview of the Credit Risk Analysis`	
	
The purpose for the the project is to employ different techniques to train and evaluate models with unbalanced classes. Also, to evaluate the performance of the models and make a written recommendation on whether they should be used to predict credit risk.

The analysis consists of three technical analysis deliverables and a written report as the following: 

- Predict Credit Risk using:
  - Resampling Models;
  - The SMOTEENN Algorithm;
  - Ensemble Classifiers;
- Submit a Written Report on the Analysis.

## `Resources`	
The analysis is created using next software: Jupyter-notebook 6.3.0, Python 3.8.8, Pandas 1.2.4, machine learning libraries for Python: imbalanced-learn 0.8.1, scikit-learn 0.24.1, Visual Studio Code 1.58.0.

## `The Credit Risk Analysis Result`
Using bulleted lists, describe the balanced accuracy scores and the precision and recall scores of all six machine learning models.
### `- Resampling Models to Predict Credit Risk`	

Using 
evaluate three machine learning models by using resampling to determine which is better at predicting credit risk. First, you’ll use the oversampling RandomOverSampler and SMOTE algorithms, and then you’ll use the undersampling ClusterCentroids algorithm. Using these algorithms, you’ll resample the dataset, view the count of the target classes, train a logistic regression classifier, calculate the balanced accuracy score, generate a confusion matrix, and generate a classification report 

The result of Resampling Models can be found in the [Credit_Risk_Resampling](./credit_risk_resampling.ipynb) file.


### `- The SMOTEENN algorithm to Predict Credit Risk`

Using your knowledge of the imbalanced-learn and scikit-learn libraries, you’ll use a combinatorial approach of over- and undersampling with the SMOTEENN algorithm to determine if the results from the combinatorial approach are better at predicting credit risk than the resampling algorithms from Deliverable 1. Using the SMOTEENN algorithm, you’ll resample the dataset, view the count of the target classes, train a logistic regression classifier, calculate the balanced accuracy score, generate a confusion matrix, and generate a classification report.

The result of the SMOTEENN algorithm can be found in the [Credit_Risk_Resampling_Models](./credit_risk_resampling.ipynb) file.

### `- Ensemble Classifiers to Predict Credit Risk`
Using your knowledge of the imblearn.ensemble library, you’ll train and compare two different ensemble classifiers, BalancedRandomForestClassifier and EasyEnsembleClassifier, to predict credit risk and evaluate each model. Using both algorithms, you’ll resample the dataset, view the count of the target classes, train the ensemble classifier, calculate the balanced accuracy score, generate a confusion matrix, and generate a classification report

The result of the SMOTEENN algorithm can be found in the [Credit_Risk_Ensemble_Classifiers](./credit_risk_ensemble.ipynb) file.

## `The Credit Risk Analysis Summary`

According to the result of the Bias ...

Summarize the results of the machine learning models, and include a recommendation on the model to use, if any. If you do not recommend any of the models, justify your reasoning.

Additionally, 
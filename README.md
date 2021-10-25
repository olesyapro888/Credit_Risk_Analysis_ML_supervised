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
	
The purpose for the project is to employ different techniques to train and evaluate models with unbalanced classes. Also, to evaluate the performance of the models and make a written recommendation on whether they should be used to predict credit risk.

The analysis consists of three technical analysis deliverables and a written report as the following: 

- Predict Credit Risk using:
  - Resampling Models;
  - The SMOTEENN Algorithm;
  - Ensemble Classifiers;
- Submit a Written Report on the Analysis.

## `Resources`	
The analysis is created using next software: Jupyter-notebook 6.3.0, Python 3.8.8, Pandas 1.2.4, machine learning libraries for Python: imbalanced-learn 0.8.1, scikit-learn 0.24.1, Visual Studio Code 1.58.0.

## `The Credit Risk Analysis Result`
### `- Resampling Models to Predict Credit Risk`	

Using Resampling Models algorithms, the dataset were resampled, the count of the target classes were viewed, a logistic regression classifier were trained, the balanced accuracy score was calculated, a confusion matrix, and a classification report were generated.

The result of Resampling Models can be found in the [Credit_Risk_Resampling](./credit_risk_resampling.ipynb) file.

According the results of three machine learning models as Random Oversampling, SMOTE Oversampling, Undersampling it may be determined as the SMOTE Oversampling model is a slightly better to predict credit risk.

Naive Random Oversampling technique like some instances of the minority class are randomly selected and added to the training set until the majority and minority classes are balanced. The accuracy score of Naive Random Oversampling is 67.4%. It means that every single observation in the testing set of Naive Random Oversampling model was correct 67.4% of the time.

![image](https://user-images.githubusercontent.com/68247343/138608730-0493ed00-0cb2-4602-bc3e-660910193598.png)

SMOTE Oversampling (the synthetic minority oversampling) technique like the size of the minority is increased. SMOTE generate synthetic observation. This model achieved an accuracy score of 66.2%.

![image](https://user-images.githubusercontent.com/68247343/138608737-7276333c-5d5f-4947-a8f0-ca87555beb25.png)

Undersampling as the size of the majority class is decreased to the size of the minority class. Undersampling model was correct 64,4% of the time.

![image](https://user-images.githubusercontent.com/68247343/138608743-6ba0a1cd-f9c8-4514-887d-906e4cc31592.png)

Even the accuracy score can be high it can be misleading, especially in an unbalanced dataset.

Precision is the measure of how reliable a positive classification is.
The results of precision are the same for three models for high_risk: 0.01 and low_risk: 1.
So, a positive classification is not reliable for high_risk and for three models.

Recall is the ability of the classifier to find all the positive samples.	
Recall ("rec" column) of Naive Random Oversampling is following: 

![image](https://user-images.githubusercontent.com/68247343/138608650-a860fcdb-b1a8-43d2-b0ee-69254f4a9310.png)

The metrics of the minority class (precision, recall, and F1 score) of the SMOTE are slightly improved.

![image](https://user-images.githubusercontent.com/68247343/138608658-f6087ba0-3d9d-4792-b488-3852b49c0eb5.png)

The results of Undersampling are unimpressive and worse than those from Naive Random Oversampling and SMOTE models.

![image](https://user-images.githubusercontent.com/68247343/138608661-6fa9e49d-b694-42e2-9a66-6c6b3d89b5f4.png)

### `- The SMOTEENN algorithm to Predict Credit Risk`

The result of the SMOTEENN algorithm can be found in the [Credit_Risk_Resampling_Models](./credit_risk_resampling.ipynb) file.

Using a combinatorial approach of over- and undersampling with the SMOTEENN algorithm it can be determined that the results from the combinatorial approach are better at predicting credit risk than the resampling algorithms from "Resampling Models" above. 

SMOTEENN combines the SMOTE and Edited Nearest Neighbors (ENN) algorithms. This model achieved an accuracy score of 66.1%.
Resampling with SMOTEENN did not work miracles, but some of the metrics show an improvement over undersampling.

![image](https://user-images.githubusercontent.com/68247343/138608309-c7701bee-1acf-4575-b4c0-466034753a41.png)
### `- Ensemble Classifiers to Predict Credit Risk`
The result of the Ensemble Classifier algorithm can be found in the [Credit_Risk_Ensemble_Classifiers](./credit_risk_ensemble.ipynb) file

To predict credit risk and evaluate each model two different ensemble classifiers, BalancedRandomForestClassifier and EasyEnsembleClassifier were trained and compared. Also,  using both algorithms, the dataset was resampled, the count of the target classes was viewed, the ensemble classifier was trained, the balanced accuracy score was calculated, a confusion matrix, and a classification report were generated.

The Balanced Random Forest Classifier model achieved an accuracy score of 78.5%.

![image](https://user-images.githubusercontent.com/68247343/138608322-585ff9af-ef94-4b50-86db-552e14b55655.png)

Easy Ensemble AdaBoost Classifier model achieved an accuracy score of 93.1%

![image](https://user-images.githubusercontent.com/68247343/138608328-4712f2c0-52b2-45f9-b3eb-065de7aaf881.png)

The metrics of the minority class (precision, recall, and F1 score) of the Easy Ensemble AdaBoost Classifier are improved.
So, the Easy Ensemble AdaBoost Classifier can be regarded as the best model to Predict Credit Risk.

## `The Credit Risk Analysis Summary`

Using six models algorithms, the dataset were resampled, the count of the target classes were viewed, a logistic regression classifier were trained, the balanced accuracy score was calculated, a confusion matrix, and a classification report were generated.

According the results of machine learning models as Random Oversampling, SMOTE Oversampling, Undersampling it may be determined as the SMOTE Oversampling model is a slightly better to predict credit risk.

Additionally, resampling with SMOTEENN did not work miracles, but some of the metrics show an improvement over undersampling.

The metrics of the minority class (precision, recall, and F1 score) of the Easy Ensemble AdaBoost Classifier are improved.
So, the Easy Ensemble AdaBoost Classifier can be regarded as the best model to Predict Credit Risk.

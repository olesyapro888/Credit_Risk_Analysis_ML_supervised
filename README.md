# Credit Risk Analysis. Project 17 of the UofT.
## `-Contents-`	
	
- [Overview of the Credit Risk Analysis](#Overview-of-the-Credit-Risk-Analysis)	
- [Resources](#resources)	
- [The Credit Risk Analysis Result](#The-Credit-Risk-Analysis-Result)
  - [ETL on Amazon Product Reviews](#--ETL-on-Amazon-Product-Reviews)
  - [Bias of Vine Reviews](#--Bias-of-Vine-Reviews)
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
### `- ETL on Amazon Product Reviews`	

Using 
The result of the ETL process on Amazon Product Reviews can be found in the [Amazon_Reviews_ETL](./Amazon_Reviews_ETL.ipynb) file.


### `- Bias of Vine Reviews`

The result of the Bias of Vine Reviews can be found in the [Vine_Review_Analysis](./Vine_Review_Analysis.ipynb) file.


## `The Credit Risk Analysis Summary`

According to the result of the Bias of Vine Reviews the number of Vine reviews is 18 and non-Vine reviews is 7652.

Additionally, "5-star Vine" reviews and "5-star non-Vine" reviews are 9 and 4376 respectively.

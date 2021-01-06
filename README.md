# Corporate-Defaults---ML-Models in Python
## One-year probability of default models that combine structural and ML methods

This project helps to determine whether the inclusion of the structural probability of default from the Merton model (PD) as an explanatory variable in classification models would improve the prediction of bankruptcy of the company. 
To conduct the study, I used the balance sheet data and quotations of American companies from the non-financial sector for the years 1985–2019 taken from the Compustat database. 
The information on corporate insolvency was obtained from the UCLA LoPucki database. 

The following classifiers were used in the study:
<li> Quadratic Discriminant Analysis
<li> Naive Bayes
<li> Logistic Regression
<li> Decision Trees
<li> Random Forest
<li> AdaBoost
<li> XGBoost
<li> Support Vector Machine
<li> K-nearest neighbors
<li> Multilayer perceptron

On the basis of the obtained results, there are no grounds to claim that the inclusion of the PD variable obtained from the Merton model significantly improves the predictive abilities of the models. 
For some classifiers, the mean ROC-AUC of the model with the PD variable is only slightly higher than the models without the PD variable, and the tests performed showed no statistical similarity of the ROC-AUC models for the significance level of 0.01, 0.05, 0.1. 
Nevertheless, the conducted study and literature research suggest that the procedure of selecting variables and number of variables may have the greatest impact on the rejection of a hypothesis. 
For this reason, it is suggested to re-conduct the study based on the step-wise selecetion algorithm. Code using this algorithm is also available in this notebook.

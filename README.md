# Malicious-Server-Hack
The dataset is on [Kaggle](https://www.kaggle.com/datasets/lplenka/malicious-server-hack). The work is to build a predictive model which can identify a pattern in 
these variables and suggest that a hack is going to happen so that the cybersecurity can somehow stop it before it actually happens. 
And I have to predict the column **MALICIOUS_OFFENSE**.

In this kernel, I use [XGBoost](https://xgboost.readthedocs.io/en/stable/), which performance is very good on test data splitting from Train.csv. With XGBOOST, we don't need to scale or normalize data.
I use [KNN imputer](https://scikit-learn.org/stable/modules/generated/sklearn.impute.KNNImputer.html) to complete missing data (X_12 column), and use [SMOTE](https://imbalanced-learn.org/stable/references/generated/imblearn.over_sampling.SMOTE.html/) 
to resample training data because the label is imbalance.

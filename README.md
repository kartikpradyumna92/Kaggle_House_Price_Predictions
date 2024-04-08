# <p style="text-align: center;"> Kaggle House Price Predictions</p>
<br>Housing price predictions on the Kaggle Housing dataset<br>
#### <b>Data Link</b> - https://www.kaggle.com/datasets/harishkumardatalab/housing-price-prediction

### <b>About the Data:</b><br>
The housing data is multi-variable data and a few features are correlated with each other, hence suffering with multicollinearity. 
<br><br>
### <b>Approach:</b><br>
We tried removing multicollinearity using the Variance Inflation Factor (VIF) but it has a few challenges. The problem is identifying the appropriate way to unify multiple fields to capture the importance of the multiple fields into one and drop those individual fields. We got a weak prediction using this method
Rescaling using MinMaxScaler on VIF data also did not result in good predictions.
This concluded our attempt to reduce dimension to avoid multicollinearity and fit the linear regression model. <br>
We used Lasso and Ridge regression since they handle multi-variable data well and deal with multicollinearity well.<br>
In addition, I used GridSearch CV to identify the best hyperparameter to use to build, fit, and predict using the model.<br><br>
This improved the accuracy and achieved <b>r2 score = 0.7092047042418796</b> on the test data.
<br><br>
#### <b>Python Packages:</b><be>
```
sklearn==1.2.2
matplotlib==3.8.4
pandas==2.2.1
numpy==1.26.4
seaborn==0.13.2
statsmodels==0.14.1
```
#### <b>Kaggle Notebook</b> - https://www.kaggle.com/code/kartikpradyumna92/housing-price-prediction

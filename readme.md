# installation 

To install requirements used to run the included notebooks run 

```
pip3 install -r requirements.txt 
```

# Discussion 

First model we thaught to use was XGBoost. Not only beacause XGBoost has a great success rate within ML competitions but because of it's feature scoring properties allowing us to filter out low scoring features for our next models. 


# Results 

![Alt text](https://github.com/TheBugMaker/Kaggle-house-prices/raw/master/kaggle.png "Model results")
![Alt text](https://github.com/TheBugMaker/Kaggle-house-prices/raw/master/kaggle%20ranking.png "Model raking results")

# Conclusion 

* The models that did best are XGBoost and LASSO which are the ones least sensitive to uncorrelated features. 
* LASSO with cross-validation (LassoCV) had the best performances probably for the fact that a linear combinaisation of the features is a good choice for a model since logically one can expect many linear correlations between the price and features such as overallQual ( the linear correlation is observed in the notebook )
* LASSO with cross-validation (LassoCV) success can also be attributed to the principled way for the choice of hyperparameters ( cross-validation ) a method which was not implemented for the other models

# House-Prices-Predictions
Developed a model that can predict the estimated market value of each home and serve as a second opinion to compare with the appraiser's value.

#**1. Introduction**

According to the National Association of Realtors, of the 75% of contracts with settlement contingencies, 41% involved appraisal issues.

In addition, according to the Realtors Confidence Index Survey, 21% of realtors say appraisal issues delayed their sales contracts in October 2020. As a result, appraisal issues led to 13% of contracts being terminated. 

**Problem:** An inaccurate appraisal can lead to a cancelled sales contract and transaction delays because lenders won’t approve mortgages for more than the home’s value.

**Solution:** the solution will be to create a model that can accurately predict the estimated market value of each home and serve as a second opinion to compare with the appraiser's value.

This price estimate should help you protect against the appraiser’s mistake and obtain accurate home prices based on market data.

# **2. Data**

The original dataset is called House Prices - Advanced Regression Techniques and was downloaded from Kaggle website: [House Prices](https://www.kaggle.com/c/house-prices-advanced-regression-techniques/data?select=train.csv). 

The data contains variables describing the aspect of residential homes. It contains 11460 observations and 81 variables.

# **3. Methodology**

**Data Cleaning:** In this step, I will eliminate any problems from the dataset which would prevent further analysis.

**Data Exploration:** In this step, I will apply statistics and visualization techniques to gain a better understanding of the dataset.

**Feature engineering:** In this final step of Exploratory Data Analysis (EDA), I will select the most useful features or create new features from the existing ones.

**Modelling:** Apply several models to predict the number of sales and select the best performing model.

#**4. Results**

The numerical features with high feature importance score and at the same time are highly correlated with the Sale Price were selected: OverallQual, YearBuilt, YearRemodAdd, BsmtFinSF1, TotalBsmtSF, 1stFlrSF, GrLivArea, Fireplaces, GarageCars, GarageArea. 
The categorical features that exhibit high variance with respect to the Sale Price were selected: Neighborhood, ExterQual, BsmtQual, KitchenQual, GarageFinish, Foundation, HeatingQC, BsmtFinType1, MasVnrType, GarageType.
Based on the R-squared, MAE, MSE, and RMSE values Gradient Boosting solution is the top performer.


# **5. Discussion & Recomendations**

From this model, interested parties will be able to compare the sale price of a house with the appraiser’s estimation to avoid cancelled sales contract and transaction delays.

The model’s sale price value is based on comparable homes in the area since the increase or decrease in price is largely based on how a house compares to others in an area. Therefore, the model’s prediction is expected to be better than the appraisers. If interested parties notice large inconsistencies between both the model and appraiser estimations; they should bring them to the attention of the real estate agent and mortgage lender.

Moreover, this model could serve as concrete evidence that the appraisal is wrong. Without a solid case, lenders will not be likely to help. However, with concrete factual backup, a lender may be able to order a new appraisal, and may even have the ability to override the first home appraisal report.

After all, an appraisal is just the appraiser’s opinion; and this model could serve as a second appraiser or opinion for comparison purposes.

House prices can be affected by economic activity. Thus, as further analysis, it is recommended to measure and integrate the interest rates in the prediction at the time houses are sold. 


# **References**

1. https://cdn.nar.realtor/sites/default/files/documents/2020-10-realtors-confidence-index-11-19-2020.pdf

2. https://www.nar.realtor/

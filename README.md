# House-Prices-Advanced-Regression-Techniques

## EDA

1.Removing columns that contain the same value in 100% ["Street", "Utilities"] <br>
2.Removing outliers : GrLivArea more than 4500.<br>
3.Improving values like Year more than 2017.<br>
4.Handling missing numerical values:<br>
- LotFrontage according to median in specific Neighborhood
* With constant = 0 for : ['BsmtFinSF1', 'BsmtFinSF2', 'BsmtFullBath', 'BsmtHalfBath', "MasVnrArea"]<br><br>
5. The rest of numerical columns (apart from point 5) with median.<br>
6. Transformation of some numerical features that are actually categorical: ['MSSubClass', 'OverallCond’]
7. Handling missing categorical values. (specific for each feature)
- Transformation of skewed features:
* SalePrice – log transformation
- Other features with skeweness > 0.5 using BoxCox transformation
* Transformation some categorical features (with specific order) into numerical <br>

## Feature Engineering:
1. Feature Isgarage defined according to feature GarageArea (1 – if more than 0)
2. Feature Isfireplace defined according to feature Fireplaces (if more than 0)
3. Feature Ispool defined according to feature PoolArea (if more than 0)
4. Feature Issecondfloor defined according to feature 2ndFlrSF (if more than 0)
5. Feature IsOpenPorch defined according to feature OpenPorchSF (if more than 0)
6. Feature IsWoodDeck defined according to feature WoodDeckSF (if more than 0)
7. Feature TotalSqrtFeet defined as sum of GrLivArea and TotalBsmtSF
8. Feature TotalBaths defined as BsmtFullBath + FullBath + BsmtHalfBath/2 + HalfBath/2.
9. One-Hot Encoding for categorical data <br>

## Modelization

1. Linear Regression
2. LASSO model selection
3. GradientBoostingRegressor
4. XGBRegressor

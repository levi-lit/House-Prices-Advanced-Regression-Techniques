# House-Prices-Advanced-Regression-Techniques

EDA
Removing columns that contain the same value in 100% ["Street", "Utilities"]
Removing outliers : GrLivArea more than 4500.
Improving values like Year more than 2017.
Handling missing numerical values:
LotFrontage according to median in specific Neighborhood
With constant = 0 for : ['BsmtFinSF1', 'BsmtFinSF2', 'BsmtFullBath', 'BsmtHalfBath', "MasVnrArea"]
The rest of numerical columns (apart from point 5) with median.
Transformation of some numerical features that are actually categorical: ['MSSubClass', 'OverallCond’]
Handling missing categorical values. (specific for each feature)
Transformation of skewed features:
SalePrice – log transformation
Other features with skeweness > 0.5 using BoxCox transformation
Transformation some categorical features (with specific order) into numerical

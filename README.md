# house_price_prediction
## Problem Statement
Problem Statement A US-based housing company named Surprise Housing has decided to enter the Australian market. The company uses data analytics to purchase houses at a price below their actual values and flip them on at a higher price. The company is looking at prospective properties to buy to enter the market. We need to predict the actual value of the prospective properties and decide whether to invest in them or not.

The company wants to know:

Which variables are significant in predicting the price of a house, and How well those variables describe the price of a house.
## Business Goal
You are required to model the price of houses with the available independent variables. This model will then be used by the management to understand how exactly the prices vary with the variables. They can accordingly manipulate the strategy of the firm and concentrate on areas that will yield high returns. Further, the model will be a good way for management to understand the pricing dynamics of a new market.
## Basic Information
- Remove unwanted columns -MSSubClass -Street -Utilities -Condition2 -RoofMatl -LowQualFinSF -ScreenPorch -EnclosedPorch -3SsnPorch -PoolArea -MiscVal
- NA treatment -Alley -FireplaceQu -PoolQC -Fence -MiscFeature -LotFrontage -Electrical -GarageType -GarageFinish -GarageQual -GarageCond -GarageYrBlt -BsmtQual -BsmtCond -BsmtExposure -BsmtFinType1 -BsmtFinType2
- Outlier treatment
## Exploratory Data Analysis
- In the first graph we can see that FV (Floating village residential) seems to be higher in price followed by RL(Low residential density)
- Top right corner graph shows the shape of the property, IR1(Slightly irregular), IR2(Moderately irregular) and IR3(Irrugular) has higher price than the Regular shaped property.
## Prediction and Evaluation
- R2_Score on train set:0.9034267539833389
- R2_Score on test set: 0.8804515883386272
## Final Model
Final Model :  -0.136 + 0.046*LotArea + 0.159*OverallQual + 0.026*OverallCond + 0.013*YearRemodAdd + 0.037*MasVnrArea + 0.054*ExterQual + 0.004*BsmtQual + 0.032*BsmtExposure + 0.088*BsmtFinSF1 + 0.004*TotalBsmtSF + 0.002*HeatingQC + 0.037*1stFlrSF + 0.266*GrLivArea + 0.013*HalfBath + 0.04*KitchenQual + 0.029*GarageCars + 0.028*GarageArea + 0.012*WoodDeckSF + 0.015*OpenPorchSF + 0.009*RL + 0.005*IR2 + 0.012*CulDSac + 0.002*Mod + 0.003*BrkSide + 0.016*Crawfor + 0.019*NoRidge + 0.034*NridgHt + 0.004*Somerst + 0.038*StoneBr + 0.012*Norm + 0.006*1Story + 0.01*Hip + 0.012*BrkFace + 0.006*CemntBd + 0.004*VinylSd + 0.011*Stone + 0.01*PConc + 0.014*Typ + 0.002*Gd + 0.009*BuiltIn + 0.004*Y + 0.05*New + 0.006*Normal


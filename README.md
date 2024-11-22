# California-Housing-Price-Prediction

Utilizing the California Housing Dataset from Scikit Learn, this project applied a Random Forest Regressor (RFR) and a Support Vector Regressor (SVR) to predict the target variable.

The dataset was created from the 1990 United States Census Bureau and consists of eight numeric features and the target variable. The features and target are as follows:

Total instances: 20640
• MedInc median income in block group
• HouseAge median house age in block group
• AveRooms average number of rooms per household
• AveBedrms average number of bedrooms per household
• Population block group population
• AveOccup average number of household members
• Latitude block group latitude
• Longitude block group longitude
• Target house price

*A block group is the smallest geographical unit used and publisheb by the US Census Bureau

In addition to the RFR and SVR models, this project contains three additional features; a user input function to predict a singular house price based off input, a renovation calculator, which predicts a home's value plus the percent increase in value post renovations, and a rent calculator, which predicts a given home's predicted rent price. 

The RFR model was built using the ensemble module from the sklearn library with 500 estimators and a random state of 42 for reproducibility. The model's cross validator was 5-fold and used R-squared for scoring. Model evaluation was completed using root mean squared error, mean absolute error, and R-squared. Feature importance was plotted as a visual aid and the model's actual versus predicted values were shown in a scatterplot with a regression line. 

The SVR was built using the svm module from the sklearn library. The model was defined with the non-linear radial basis function kernel, a regularization parameter of 100, and epsilon set to 0.1 for a balance between precision and robustness. The evaluation metrics for the model were root mean suqared error, mean absolute error, and R-squared. The actual versus predicted values were plotted as a scatterplot with a regression line for visualization. 

The user input for base housing price was a singular function designed to allow data related to a specific home be input and a predicted house price be returned. 

The renovation calculator was built off the aforementioned function and designed to take both a home's specific data and renovation type to return the base price and a price reflecting the value increase from renovations. The renovation data used by the function was written directly into the notebook as a dataframe and is not an additional data file. 

The rent calculator was designed to predict the rent of a singular home BY......

Contributors: Kiera Wingo, Fidel Gonzalez, Prashant Vajpayee, and Komala Cherukuri

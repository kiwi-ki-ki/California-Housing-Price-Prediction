# California-Housing-Price-Prediction

Utilizing the California Housing Dataset from Scikit Learn, this project applied a Random Forest Regressor (RFR) and a Support Vector Regressor (SVR) to predict the target variable.

The dataset was created from the 1990 United States census by and consists of eight numeric features and the target variable. The feature and target are as follows:

Total instances: 20640
• MedInc median income in block group
• HouseAge median house age in block group
• AveRooms average number of rooms per household
• AveBedrms average number of bedrooms per household
• Population block group population
• AveOccup average number of household members
• Latitude block group latitude
• Longitude block group longitude

*A block group is the smallest geographical unit used and publiches by the US Census Bureau

In additional to the RFR and SVR models, this project contains additional features including a user input function to receive a house price for a singular and specific home, a renvation calutalor, which predicts a home's value plus the percent increase in value post renovations, and a rent calculator, which predicts a given home's predicted rent price. 

The RFR model was built using the ensemble module from the sklearn library with 500 estimators and a random state of 42 for reproducibility. The model's cross validator was 5-fold and used R-squared for scoring. Model evaluation was completed using root mean squared error, mean absolute error, and R-squared. Feature importance was plotted as a visual aid and the model's actual versus predicted values were shown in a scatterplot with a regression line. 

The SVR was built using the svm module from the sklearn library. The model was defined with the non-linear radial basis function kernel, a regularization parameter of 100, and epsilon set to 0.1 for a balance between precision and robustness. The evaluation metrics for the model were root mean suqared error, mean absolute error,. and R-squared. The actual versus predicted values were plotted as a scatterplot with a regression line for visualization. 

The user input for base housing price was a singular function designed to allow data related to a specific home top be input and a predicted house price be returned. 

The reonvation calculator was designed to build off of the base housing prediction function and return a predited house price that took the home's specifications, plus the type of renovation perfromed, and return a new home price. The additional renovation data was built directly into the notebook and is not an additional data file. 

The rent calculator was designed to predict the rent of a singular home BY......

Contributors: Kiera Wingo, Fidel Gonzalez, Prashant Vajpayee, and Komala Cherukuri

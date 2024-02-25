Hi!

This is a basic project demonstrating the use of Supervised Learning to predict car selling prices for city cars depending on the kilometers driven and the year using Linear Regression the scikit-learn framework in a jupyter notebook environment.

The CSV-dataset is publicly available and was downloaded from https://www.kaggle.com/datasets/nehalbirla/vehicle-dataset-from-cardekho/discussion

To rebuild this project, you'll need the following libraries:
- Pandas
- sklearn
(- matplot)

This is the thinking concept I used for this project:
1. Use pandas to transform the CSV into a dataframe and inspect the 'Car_Name' column for the most represented car model which is the "city" model
2. "Clean" the data by creating a new dataframe for only the city cars
3. Use matplot diagrams to see how the year and kms driven influence the selling price
4. Take these two as features for the model and selling price as the depending variable we want to predict
5. Train and test the model with Linear Regression using scikit-learn methods
6. Test the model's quality using the r2-score method from scikit-learn

For extra functionality, I wanted to use the model to allow a buyer like a car dealer to enter a year and kilometers driven to use the models prediction as a starting point for the negotiation:
1. Define a function, inside the function define two variables using the python input method to capture the inputs for the year and kilometers
2. Still inside the function, transform the results into a dataframe 
3. Then use the built model to predict the price given the dataframe as parameter and store the result in a variable, that should be returned by the function
4. Output the functions result (the price prediction) using a f-string print statement

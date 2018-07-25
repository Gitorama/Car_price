  I predicted the price(MSRP) of a car from features such as the amount of horsepower, miles per gallon in the city and highway, and the weight
of the car. I obtained the dataset from Kaggle.com which consisted of different car makes, models, MSRP, horsepower, etc., the dataset had 428 rows and 15 columns. I first cleaned the data by replacing null values, making sure that the values in each of the columns were of the correct datatype, and then deleting certain columns(such as string columns) that wouldn't have anything to do with predicting my target column - The MSRP. I went ahead I deleted 5 rows as I realized that they were outliers in my Data. I ended up with 423 rows and 8 columns after cleaning my data. 

Next, I generated a heatmap of all my features along with the target(my MSRP) so that I could see the correlations. I decided to go ahead and use all of my features(Engine size, Number of Cylinders, horsepower, MPG_City, MPG_Highway, Weight, Wheelbase, and Length), along with my target as it gave me the highest cross-validation score. I ended up bootstrapping the dataset from 425 rows to 1000 rows so that I would have ample sizes for my training and test data. I used Sklearn's resample function in order to bootstrap my dataset to 1000 rows, and then I split the Data up into 80% training Data and 20% test data. I used Multi-linear Regression and Random Forest Regression to train my models but ended up going with Random Forest Regression as it gave me the highest prediction accuracy of around 97% and a low mean-squared error of .023. 

Some of the results that surprised me were the fact that Porsches were the most expensive cars on average, that Cadillacs were the most expensive American cars on average, and that the Dodge Viper SRT-10 Convertible had the most horsepower than any other car of close to 500hp. 





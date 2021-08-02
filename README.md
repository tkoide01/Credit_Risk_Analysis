# Credit_Risk_Analysis

## Overview of Project

### Purpose



## Results:
#### Naive Random Oversampling:
+ The below VBA code is built to output Ticker, Totaly Daily Volume, and Return of each stock. Also, the code compiles functions to format the output code and report its execution time; 

   ![](images/1_random_oversampling.png)

#### SMOTE oversampling:
2. Enter the worksheet's title and headers for tables. Note that `Worksheets("All Stocks Analysis").Activate` code is there to ensure the table is created on the worksheet "All Stocks Analysis" that we want to report.

   ![](images/2_SMOTE.png)

#### Cluster Centroids undersampling:
3. Initialize array of all 12 tickers.
   
   ![](images/3_clustercentroids.png)
   
#### SMOTEENN Combination(over and under) sampling:
4. Create and initialize the variables `tickerIndex`  and output arrays `tickerVolume, tickerStartingPrices,` and `tickerEndingPrices` to organize the upcoming code.
   
   ![](images/4_SMOTEENN.png)
   
#### Balanced Random Forest Classifier:
5. Write `for` loop and `If Then` codes to determine `tickerVolume, tickerStartingPrices,` and `tickerEndingPrices`. 

   
   ![](images/5_BalancedRandomForestClassifier.png)
   
#### Easy Ensemble AdaBoost Classifier:
6. Write the formula to output Ticker, Total Daily Volume, and Return to the table.
   
   ![](images/6_EasyEnsembleClassifier.png)
   

## Summary:

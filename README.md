# Neural_Network_Charity_Analysis

## Overview of the analysis

The purpose of this project was to train a supervised learning model on loan data and see the accuracy in predicting if applicants will be successful if funded by Alphabet Soup.
The dataset consisted of 12 columns of data.  Tensorflow within Python was used to develop the model.  An image of the dataset.

<img width="811" alt="image" src="https://user-images.githubusercontent.com/85581208/157491951-b40c781c-a29e-427a-b4a7-09b264516bf5.png">

The EIN and NAME columns were dropped from the dataframe.  Then two categories were examined for binning, APPLICATION_TYPE and CLASSIFICATION.  Using a density plot a value was used to create new bins for both columns to help with the accuracy of the model.  OneHotEncoder was utilized to fit and transform the categorical variable list.  Code shown in image below.

<img width="684" alt="image" src="https://user-images.githubusercontent.com/85581208/157494247-9748b30d-c9bb-4889-8c02-6b1e071de3c2.png">

Then the original dataframe plus the encode_df were merged before splitting the data into features and target arrays.  The data was then scaled and the model built and run.



## Results
  
  -Data Preprocessing
    -  The target of the model is the IS_SUCCESFUL data
    -  The features are all values within the dataframe except the IS_SUCCESSFUL data
    -   Variables that are removed are the EIN and NAME.  They do not determine theh outcome of whether or not the funding is successful.
   
  - Compiling, Training, and Evaluating the Model
    -I selected 8 nodes for the first hidden layer and no other layers after multiple runs.  When I lowered or raised the number of nodes in the first layer from 8 the accuracy      score went down.  Using only one layer gave me the best results.
    
    -The target model performance was not achieved.  The original accuracy was 0.569. In the optimization file the accuracy score was raised to 0.722.  Just slightly under the       target of 0.75 or 75%.
    
    -Steps taken to increase the model performance included binning the INCOME_AMT feature due to the enormous range of numbers.  One attempt included dropping the                   SPECIAL_CONSIDERATIONS column but this had no affect.  Multiple runs with different node amounts and a second layer and third layer of nodes.  The activation type was           changed to elu but this did not improve the accuracy score.  It decreased it.
    




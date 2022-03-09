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
    -  




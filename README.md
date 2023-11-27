# Deep-Learning-Challenge
  # Preprocess the Data

    To process the Data I started with dropping the EIN and NAME columns from the DataFrame since they were not beneficial to use in what I wanted to acheive.  After that I looked for the number of unique values in each column and then set my cutoff to 10 unique values so that the most relevant will show and the outliers or ones that do not show up as much are filtered out.  After I filtered my unique values I converted my new data into a new DataFrame using Get Dummies.  Then to split my data into fetures and target arrays I made my y variable equal the "IS_SUCCESSFUL" values and my x variable to be everything else.  To complete my preprocessing I used my StandardScaler to trasnform the data and scale it. 

  # Compile, Train, and Evaluate the Model

    To complie my data to be able to evalute I used the Sequential model and set my layers to be able to run and check the structer of the model.  The outcomes I got from the model were almost all of the 627 params in the first layer being 576, and then only 45 in the second layer and 6 in the third layer.
    
  # Optimize the Model
    
    To optimize the model I used the evalute method to test the model and my loss was .5654 and accuracy was .7234.  After I had the model evaluated I exported it to a HDF5 file. 

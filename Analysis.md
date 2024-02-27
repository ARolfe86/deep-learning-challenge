1. **Overview** of the analysis:
   * The non-profit foundation Alphabet Soup wants a tool that can help it select the
     applicants for funding with the best chance of success in their ventures. With our
     knowledge of machine learning and neural networks, we will use the features in
     the provided dataset to create a binary classifier that can predict whether
     applicatns will be successful if funded by Alphabet Soup.

2. **Results**:
* Data Preprocessing
    * What variable(s) are the target(s) for your model?
      
      * In this case we will use "IS_SUCCESSFUL" variable as our target, as it is the
             main indicator to see if the money will be used efficiently after applying our model.
    * What variable(s) are the features for your model? The rest of the data, excluding 
      "**EIN**" and "**NAME**" will be used as our features:

      * **APPLICATION_TYPE**—Alphabet Soup application type
      * **AFFILIATION**—Affiliated sector of industry
      * **CLASSIFICATION**—Government organization classification
      * **USE_CASE**—Use case for funding
      * **ORGANIZATION**—Organization type
      * **STATUS**—Active status
      * **INCOME_AMT**—Income classification
      * **SPECIAL_CONSIDERATIONS**—Special considerations for application
      * **ASK_AMT**—Funding amount requested
 
  * What variable(s) should be removed from the input data because they are neither targets nor features?
      * "**EIN**" and "**NAME**" since they were in an identification column.
   
* Compiling, Training, and Evaluating the Model
  
  * How many neurons, layers, and activation functions did you select for your neural network model, and why?
    
      * For the first model, I decided to use 2 hidden layers with 80 and 30 neurons.
  I chose 80 and 30 because as a rule of thumb; the number of neurons is normally
  2 or 3 times of the input features, which was 108 in this case.
    
  * Were you able to achieve the target model performance?
     
      * No, first model was only getting around 73% accuracy which is close to the target result 75%.
        
  * What steps did you take in your attempts to increase model performance?
    
	* I will attempt to:
	* Adjust the input data to ensure that no variables or outliers are causing confusion in the model, such as:
	* Dropping more or fewer columns.
	* Creating more bins for rare occurrences in columns.
	* Increasing or decreasing the number of values for each bin.
	* Add more neurons to a hidden layer.
	* Add more hidden layers.
	* Use different activation functions for the hidden layers.
	* Add or reduce the number of epochs to the training regimen.

 3. **Summary**:
    * After attempting various steps as mentioned above, I still could not acheive the targeted results of 75% or higher.
       I did attempt to run an auto_optimization code to create a new sequential model with hyperparameter options,
       but I was unsuccessful in getting the code to work properly. I was trying to run the kerastuner to search for the best hyperparameters,
       but again, failed. If I had more time to delve into this project, I may have found a better suited model to run to acheive the desired goal.  


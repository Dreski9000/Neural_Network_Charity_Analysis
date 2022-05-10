# Neural_Network_Charity_Analysis
Module 19 of UCB Data Science Bootcamp - Alphabet Soup Charity Analysis w/ Deep Learning

### Analysis Overview
The purpose of this analysis is to attempt to build a predictive model for charity application data; in order to predict if a funds application would be approved based on
an array of information.

### Results
 * *Data Preprocessing*
    * Target variables: IS_SUCCESSFUL (whether or not the application was approved)
    * Features: Application Type, Classification, Use Case, Organization, Status, Income Amount, Special Consideration, Ask Amount
    * Removed: EIN, Name
* *Compiling,Training, and Evaluating the Model*
    * How many layers and which activation functions were selected?
        - I experimented with 2-3 layers, and between 7 to 3 neurons per hidden layer. The number of neurons seemed to have a larger impact than number of layers. The complexity of the data did not call for more layers. Relu activation function was used for hidden layers since it has the best gradient optimization, and Sigmoid was used as output since the problem involved Binary Classification.
    * Were you able to achieve target model performance?
        - No, the target model performance of 75% accuracy was not achieved. The best accuracy achieved was 65%. 
    * Which steps did you take to try to increase the model performance?
        - I experiemented with different network paramaters; but the data set itself may not have enough salient information to reach the desired predictive ability. The entropy and covariance of the features and target parameters should be evaluated to determine if this dataset is sufficient to train a model to a degree of high accuracy.

### Summary
In conclusion, the complexity of the given dataset does not appear to warrant a deep network leanring model. A better predictive model might be Gradient Boosted or Random Forest Search supervised learning, but there may be inherent problems with the dataset itself which may hinder predictive ability.



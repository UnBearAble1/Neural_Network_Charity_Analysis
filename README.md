# Neural Network Charity Analysis

## Overview of the analysis

This analysis looked at the key metadata for over 34,000 organizations that received funding from the Alphabet Soup group, to attempt to determine what the key indicators are for groups that successfully used their funding. In the metadata, the binary classifier used for the target data was if the group was successful and other data to review included the organization name, type of application, their industry and organization type, if they were active, and the amount asked for among a handful of other categories.

## Results

### Data Preprocessing

* As mentioned above, the target variable for this analysis is if they are successful, as represented by "IS_SUCCESSFUL" on the dataset

* The targets that are features include the following:
  *   Alphabet Soup application type
** Affiliated sector of industry
** Government organization classification
** Use case for funding
** Organization type
** Active status
** Income classification
** Special consideration for application, and
** Funding amount requested

* The targets that are neither targets nor features and should be removed from the input data are EIN and NAME identification columns

### Compiling, Training and Evaluating the Model

* For the final test of the neural network, two layers were used with 100 neurons in the first layer and 40 in the second. Both hidden layers used the relu activation and the output layer used a sigmoid activation. This model increased the number of neurons in the attempt to have more training to achieve better results but ultimately did not see much improvement

* Despite numerous attempts and the use of the kerastuner to attempt to find a model that would perform at the target level, we were not able to get above 75%

* As mentioned above, the kerastuner was used to try several different amounts of neurons, layers and activation functions. When none of those were able to meet the results, per the guidelines, three different set ups with varying parameters were tried but all returned approximately the same results

## Summary

Overall, the machine learning model did not achieve above a 75% accuracy and was not able to provide insight into predicting which groups would be able to successfully spend their funding amounts in the future. For ny future analysis, I would recommend having more data points that can be included or potentially reducing some of the features and eliminating noise that might be confusing the results


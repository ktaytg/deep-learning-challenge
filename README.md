# deep-learning-challenge

The nonprofit foundation Alphabet Soup wants a tool that can help it select the applicants for funding with the best chance of success in their ventures. With your knowledge of machine learning and neural networks, you’ll use the features in the provided dataset to create a binary classifier that can predict whether applicants will be successful if funded by Alphabet Soup.

## Results
# Data Preprocessing
* What variable(s) are the target(s) for your model?
  The target variable for this model will be the "IS_SUCCESSFUL" category, we train our model to identify if the campains will be successful.

* What variable(s) are the feature(s) for your model?
  The feature variables are all other columns/categories (except for EIN and NAME).

* What variable(s) should be removed from the input data because they are neither targets nor features?
  In our model, we removed EIN & NAME categories because they were not targets or features.

# Compiling, Training, and Evaluating the Model

* How many neurons, layers, and activation functions did you select for your neural network model, and why?
  In the first model, these were the recommended settings based on the output provided in the starter code.  This model achieved an accuracy score of 72.46%
  hidden_nodes_layer1 = 80
  hidden_nodes_layer2 = 30

  I tried the same model with switching all but the first layer to sigmoid activation functions, accuracy inceased as 73.33%.

Tried below model achieved an accuracy score of 72.87%
hidden_nodes_layer1 = 80
hidden_nodes_layer2 = 10
  
* What steps did you take in your attempts to increase model performance?
For my first optimization model, I added a third layer with 5 nodes,I switched all but the first layer to sigmoid activation functions. This model achieved a 72.78% accuracy.
hidden_nodes_layer1 = 85
hidden_nodes_layer2 = 25
hidden_nodes_layer3 = 5


I switched all but the first layer to sigmoid activation functions.Removed the third layer, increase the first layer to 130 and 2nd layer to 50. This model achieved an accuracy score of 73.39%
hidden_nodes_layer1 = 130
hidden_nodes_layer2 = 50

I tried to add a layer as below but accuracy score was 73.35% which is lower than previous version
hidden_nodes_layer1 = 130
hidden_nodes_layer2 = 50
hidden_nodes_layer3 = 10

* Were you able to achieve the target model performance?
In the end, I was not able to achieve the target model performance. The closest I got was in my second optimization model with a rate of 73.39%.

## Summary
Overall, the most efficient model that I created was had an accuracy of 73.39%. 
This did not achieve the target model performance of 75% and would therefore mean that this model is not yet ready to be utilized as a trustworthy tool for this company.
To increase the effectiveness of our model, we may try removing more categories that may be too niche to generalize like "SPECIAL_CONSIDERATIONS" and we can always increase the data.

# Alphabet Soup Charity

## Project Overview

Neural Networks and Deep Learning Techniques were used to analyse data, predict outcomes and evaluate the accuracy of the model utilised.

## Resources
#### Language and Packages
* Python v 3.7.6
* Pandas v 1.0.3
* Numpy v 1.18.1
* Scikit-learn v 0.22.1
* TensorFlow v 2.0.0 (also playground.tensorflow.org)

#### Data
* [charity_data.csv](https://github.com/Alyssa-CG/Module19-Deep_Learning/blob/master/Challenge/charity_data.csv)

## Challenge 

The Challenge code can be found [here](https://github.com/Alyssa-CG/Module19-Deep_Learning/blob/master/Challenge/AlphabetSoupChallenge.ipynb).

## Challenge Questions

#### How many neurons and layers did you select for your neural network model? Why?

I decided on two layers to as it seemed appropriate for the number of inputs based on the exercises in the learning portion of the module with similar numbers of inputs.

The general rule of thumb is to use 2-3 neurons per input. I compared to a learning activity and, as the number_input_features in my model was 46, I used a proportionately higher number than in a learning activity where the number_input_features was 36.

#### Were you able to achieve the target model performance? What steps did you take to try and increase model performance?

No, I was not able to achieve 75% accuracy with my model.

To increase model performance I tried:
* Increasing the number of layers, but adding a third layer did not change the accuracy so I removed it.
* Increasing the number of nodes (doubling), but I did not want to overfit the data so I returned to the previously selected numbers.
* Changing the activation functions for the layers but ultimately remained on sigmoid, which is described as "ideal for binary classification" within the module.
* Adding additional epochs (to 500) but while the model took significantly longer to run that way, it did not improve accuracy.
![500 epochs](https://github.com/Alyssa-CG/Module19-Deep_Learning/blob/master/Challenge/Other/500%20epochs.png)

#### If you were to implement a different model to solve this classification problem, which would you choose? Why?

* For a different option for this tabular data, I would consider using a random forest instead. Random forests can achieve similar results to deep learning models, while also training on the data and predicting outcomes much faster. 
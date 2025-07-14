

- Create ML
- MLSoundClassifier
- MLSoundClassifier.ModelParameters
- MLSoundClassifier.ModelParameters.ClassifierType
-  MLSoundClassifier.ModelParameters.ClassifierType.multilayerPerceptron(layerSizes:) 

Case

# MLSoundClassifier.ModelParameters.ClassifierType.multilayerPerceptron(layerSizes:)

A neural network model that uses three or more layers to classify an input into a category.

macOS 11.0+

``` source
case multilayerPerceptron(layerSizes: [Int])
```

## Parameters 

`layerSizes`  

An array of positive integers. Each element represents the number of units for that hidden layer.

## Discussion

The neural network has a minimum of three layers:

- An input layer

- One or more hidden layers

- An output layer

The number of integers in your `layerSizes` array determines the number of hidden layers in the neural network. Each integer in the array determines the size of that hidden layer.

## See Also

### Designating an algorithm’s classifier

case logisticRegressor

A statistical model that uses logistic regression to classify an input vector into a category.


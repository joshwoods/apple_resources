

- Create ML
- MLImageClassifier
- MLImageClassifier.ModelParameters
- MLImageClassifier.ModelParameters.ClassifierType
-  MLImageClassifier.ModelParameters.ClassifierType.logisticRegressor 

Case

# MLImageClassifier.ModelParameters.ClassifierType.logisticRegressor

Logistic regression is a statistical model that classifies input feature vector into different categories.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 11.0+visionOS 1.0+

``` source
case logisticRegressor
```

## See Also

### Designating an algorithm’s classifier

case multilayerPerceptron(layerSizes: [Int])

Multilayer perceptron, layerSizes holds a list of positive integers that represent the number of hidden units in each layer. An additional fully connected layer with a Softmax activation output will be added that maps to probabilities of sound categories.


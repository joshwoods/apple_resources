

- Create ML
- MLImageClassifier
- MLImageClassifier.ModelParameters
- MLImageClassifier.ModelParameters.ClassifierType
-  MLImageClassifier.ModelParameters.ClassifierType.multilayerPerceptron(layerSizes:) 

Case

# MLImageClassifier.ModelParameters.ClassifierType.multilayerPerceptron(layerSizes:)

Multilayer perceptron, layerSizes holds a list of positive integers that represent the number of hidden units in each layer. An additional fully connected layer with a Softmax activation output will be added that maps to probabilities of sound categories.

macOS 11.0+

``` source
case multilayerPerceptron(layerSizes: [Int])
```

## See Also

### Designating an algorithm’s classifier

case logisticRegressor

Logistic regression is a statistical model that classifies input feature vector into different categories.


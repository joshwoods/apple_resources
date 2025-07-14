

- Create ML
- MLActionClassifier
-  init(trainingData:parameters:) 

Initializer

# init(trainingData:parameters:)

Creates an action classifier with a training dataset represented by a data source.

macOS 11.0+

``` source
init(
    trainingData: MLActionClassifier.DataSource,
    parameters: MLActionClassifier.ModelParameters = ModelParameters()
) throws
```

## Discussion

- trainingData: A collection of labeled images represented by a data source.


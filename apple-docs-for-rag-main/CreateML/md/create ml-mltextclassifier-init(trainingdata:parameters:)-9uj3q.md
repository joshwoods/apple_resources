

- Create ML
- MLTextClassifier
-  init(trainingData:parameters:) 

Initializer

# init(trainingData:parameters:)

Creates a text classifier.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 10.15+visionOS 1.0+

``` source
init(
    trainingData: [String : [String]],
    parameters: MLTextClassifier.ModelParameters = ModelParameters(validation: .split(strategy: .automatic))
) throws
```

## Parameters 

`trainingData`  

A dictionary specifying the training data.

`parameters`  

Model training parameters.

## See Also

### Creating and training a text classifier

init(trainingData: DataFrame, textColumn: String, labelColumn: String, parameters: MLTextClassifier.ModelParameters) throws

Creates a text classifier.

init(trainingData: MLTextClassifier.DataSource, parameters: MLTextClassifier.ModelParameters) throws

Creates a text classifier.

enum DataSource

A data source for a text classifier.

struct ModelParameters

Parameters that specify model training parameters and validation data.

let modelParameters: MLTextClassifier.ModelParameters

The configuration parameters that the text classifier used for training during initialization.

init(trainingData: MLDataTable, textColumn: String, labelColumn: String, parameters: MLTextClassifier.ModelParameters) throws

Creates a text classifier.

Deprecated


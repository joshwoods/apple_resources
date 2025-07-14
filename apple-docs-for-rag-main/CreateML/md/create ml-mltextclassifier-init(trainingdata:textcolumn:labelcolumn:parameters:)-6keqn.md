

- Create ML
- MLTextClassifier
-  init(trainingData:textColumn:labelColumn:parameters:) 

Initializer

# init(trainingData:textColumn:labelColumn:parameters:)

Creates a text classifier.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+visionOS 1.0+

``` source
init(
    trainingData: DataFrame,
    textColumn: String,
    labelColumn: String,
    parameters: MLTextClassifier.ModelParameters = ModelParameters(validation: .split(strategy: .automatic))
) throws
```

## Parameters 

`trainingData`  

A data frame specifying the training data.

`textColumn`  

The name of the text column in the provided trainingData.

`labelColumn`  

The name of the label column in the provided trainingData.

`parameters`  

Model training parameters.

## See Also

### Creating and training a text classifier

init(trainingData: [String : [String]], parameters: MLTextClassifier.ModelParameters) throws

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


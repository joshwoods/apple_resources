

- Create ML
- MLTextClassifier
-  init(trainingData:textColumn:labelColumn:parameters:) Deprecated

Initializer

# init(trainingData:textColumn:labelColumn:parameters:)

Creates a text classifier.

iOS 15.0–16.0DeprecatediPadOS 15.0–16.0DeprecatedMac Catalyst 15.0–16.0DeprecatedmacOS 10.14–13.0DeprecatedvisionOS 1.0+

``` source
init(
    trainingData: MLDataTable,
    textColumn: String,
    labelColumn: String,
    parameters: MLTextClassifier.ModelParameters = ModelParameters(validationData: nil)
) throws
```

Deprecated

Use DataSource instead of MLDataTable when initializing.

## Parameters 

`trainingData`  

A table specifying training data

`textColumn`  

Name of the text column in the provided trainingData

`labelColumn`  

Name of the label column in the provided trainingData

`parameters`  

Model training parameters.

## See Also

### Creating and training a text classifier

init(trainingData: [String : [String]], parameters: MLTextClassifier.ModelParameters) throws

Creates a text classifier.

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


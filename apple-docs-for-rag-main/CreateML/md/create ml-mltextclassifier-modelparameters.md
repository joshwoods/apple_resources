

- Create ML
- MLTextClassifier
-  modelParameters 

Instance Property

# modelParameters

The configuration parameters that the text classifier used for training during initialization.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 10.14+visionOS 1.0+

``` source
let modelParameters: MLTextClassifier.ModelParameters
```

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

init(trainingData: MLDataTable, textColumn: String, labelColumn: String, parameters: MLTextClassifier.ModelParameters) throws

Creates a text classifier.

Deprecated


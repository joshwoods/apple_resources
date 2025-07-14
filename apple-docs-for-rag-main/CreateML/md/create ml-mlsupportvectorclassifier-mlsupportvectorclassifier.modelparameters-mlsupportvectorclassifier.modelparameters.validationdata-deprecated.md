

- Create ML
- MLSupportVectorClassifier
- MLSupportVectorClassifier.ModelParameters
-  MLSupportVectorClassifier.ModelParameters.ValidationData Deprecated

Enumeration

# MLSupportVectorClassifier.ModelParameters.ValidationData

Values for specifying validation data.

macOS 10.15–14.0Deprecated

``` source
enum ValidationData
```

## Topics

### Specifying validation data

case split(strategy: MLSplitStrategy)

Generate validation data by splitting the training dataset. This is the default.

case table(MLDataTable)

Set validation data from the MLDataTable provided.

case dataFrame(DataFrame)

Validation data provided in a DataFrame.

case none

Do not set validation data.

## See Also

### Creating parameters

init(validation: MLSupportVectorClassifier.ModelParameters.ValidationData, maxIterations: Int, penalty: Double, convergenceThreshold: Double, featureRescaling: Bool)

Creates a new set of parameters.

Deprecated

init(validationData: MLDataTable?, maxIterations: Int, penalty: Double, convergenceThreshold: Double, featureRescaling: Bool)

Creates a new set of parameters.

Deprecated


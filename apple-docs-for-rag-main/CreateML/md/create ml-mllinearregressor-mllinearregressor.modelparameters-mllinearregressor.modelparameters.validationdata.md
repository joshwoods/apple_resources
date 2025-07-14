

- Create ML
- MLLinearRegressor
- MLLinearRegressor.ModelParameters
-  MLLinearRegressor.ModelParameters.ValidationData 

Enumeration

# MLLinearRegressor.ModelParameters.ValidationData

Values for specifying validation data.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 11.0+tvOS 16.0+visionOS 1.0+

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

Set validation data from the DataFrame provided.

case none

Do not set validation data.

## See Also

### Creating parameters

init(validation: MLLinearRegressor.ModelParameters.ValidationData, maxIterations: Int, l1Penalty: Double, l2Penalty: Double, stepSize: Double, convergenceThreshold: Double, featureRescaling: Bool)

init(validationData: MLDataTable?, maxIterations: Int, l1Penalty: Double, l2Penalty: Double, stepSize: Double, convergenceThreshold: Double, featureRescaling: Bool)

Creates a new set of parameters.

Deprecated


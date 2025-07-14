

- Create ML
- MLLinearRegressor
- MLLinearRegressor.ModelParameters
-  init(validation:maxIterations:l1Penalty:l2Penalty:stepSize:convergenceThreshold:featureRescaling:) 

Initializer

# init(validation:maxIterations:l1Penalty:l2Penalty:stepSize:convergenceThreshold:featureRescaling:)

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 11.0+tvOS 16.0+visionOS 1.0+

``` source
init(
    validation: MLLinearRegressor.ModelParameters.ValidationData,
    maxIterations: Int = 10,
    l1Penalty: Double = 0,
    l2Penalty: Double = 0.01,
    stepSize: Double = 1.0,
    convergenceThreshold: Double = 0.01,
    featureRescaling: Bool = true
)
```

## See Also

### Creating parameters

init(validationData: MLDataTable?, maxIterations: Int, l1Penalty: Double, l2Penalty: Double, stepSize: Double, convergenceThreshold: Double, featureRescaling: Bool)

Creates a new set of parameters.

Deprecated

enum ValidationData

Values for specifying validation data.


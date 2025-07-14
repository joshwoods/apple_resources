

- Create ML
- MLDecisionTreeRegressor
- MLDecisionTreeRegressor.ModelParameters
-  init(validation:maxDepth:minLossReduction:minChildWeight:randomSeed:) 

Initializer

# init(validation:maxDepth:minLossReduction:minChildWeight:randomSeed:)

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 11.0+tvOS 16.0+visionOS 1.0+

``` source
init(
    validation: MLDecisionTreeRegressor.ModelParameters.ValidationData,
    maxDepth: Int = 6,
    minLossReduction: Double = 0,
    minChildWeight: Double = 0.1,
    randomSeed: Int = 42
)
```

## See Also

### Creating parameters

init(validationData: MLDataTable?, maxDepth: Int, minLossReduction: Double, minChildWeight: Double, randomSeed: Int)

Creates a new set of parameters.

Deprecated

enum ValidationData

Values for specifying validation data.


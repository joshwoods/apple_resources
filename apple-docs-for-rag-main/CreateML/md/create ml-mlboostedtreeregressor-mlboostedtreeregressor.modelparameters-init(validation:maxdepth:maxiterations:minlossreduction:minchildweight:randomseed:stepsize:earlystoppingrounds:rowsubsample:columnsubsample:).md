

- Create ML
- MLBoostedTreeRegressor
- MLBoostedTreeRegressor.ModelParameters
-  init(validation:maxDepth:maxIterations:minLossReduction:minChildWeight:randomSeed:stepSize:earlyStoppingRounds:rowSubsample:columnSubsample:) 

Initializer

# init(validation:maxDepth:maxIterations:minLossReduction:minChildWeight:randomSeed:stepSize:earlyStoppingRounds:rowSubsample:columnSubsample:)

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 11.0+tvOS 16.0+visionOS 1.0+

``` source
init(
    validation: MLBoostedTreeRegressor.ModelParameters.ValidationData,
    maxDepth: Int = 6,
    maxIterations: Int = 10,
    minLossReduction: Double = 0,
    minChildWeight: Double = 0.1,
    randomSeed: Int = 42,
    stepSize: Double = 0.3,
    earlyStoppingRounds: Int? = nil,
    rowSubsample: Double = 1.0,
    columnSubsample: Double = 1.0
)
```

## See Also

### Creating parameters

init(validationData: MLDataTable?, maxDepth: Int, maxIterations: Int, minLossReduction: Double, minChildWeight: Double, randomSeed: Int, stepSize: Double, earlyStoppingRounds: Int?, rowSubsample: Double, columnSubsample: Double)

Creates a new set of parameters.

Deprecated

enum ValidationData

Values for specifying validation data.




- Create ML
- MLRandomForestClassifier
- MLRandomForestClassifier.ModelParameters
-  init(validation:maxDepth:maxIterations:minLossReduction:minChildWeight:randomSeed:rowSubsample:columnSubsample:) 

Initializer

# init(validation:maxDepth:maxIterations:minLossReduction:minChildWeight:randomSeed:rowSubsample:columnSubsample:)

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 10.15+tvOS 16.0+visionOS 1.0+

``` source
init(
    validation: MLRandomForestClassifier.ModelParameters.ValidationData = .split(strategy: .automatic),
    maxDepth: Int = 6,
    maxIterations: Int = 10,
    minLossReduction: Double = 0,
    minChildWeight: Double = 0.1,
    randomSeed: Int = 42,
    rowSubsample: Double = 0.8,
    columnSubsample: Double = 0.8
)
```

## See Also

### Creating parameters

init(validationData: MLDataTable?, maxDepth: Int, maxIterations: Int, minLossReduction: Double, minChildWeight: Double, randomSeed: Int, rowSubsample: Double, columnSubsample: Double)

Creates a new set of parameters.

Deprecated

enum ValidationData

Values for specifying validation data.


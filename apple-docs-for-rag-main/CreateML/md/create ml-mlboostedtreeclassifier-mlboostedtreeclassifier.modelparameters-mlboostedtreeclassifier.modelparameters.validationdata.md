

- Create ML
- MLBoostedTreeClassifier
- MLBoostedTreeClassifier.ModelParameters
-  MLBoostedTreeClassifier.ModelParameters.ValidationData 

Enumeration

# MLBoostedTreeClassifier.ModelParameters.ValidationData

Values for specifying validation data.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 10.15+tvOS 16.0+visionOS 1.0+

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

init(validation: MLBoostedTreeClassifier.ModelParameters.ValidationData, maxDepth: Int, maxIterations: Int, minLossReduction: Double, minChildWeight: Double, randomSeed: Int, stepSize: Double, earlyStoppingRounds: Int?, rowSubsample: Double, columnSubsample: Double)

init(validationData: MLDataTable?, maxDepth: Int, maxIterations: Int, minLossReduction: Double, minChildWeight: Double, randomSeed: Int, stepSize: Double, earlyStoppingRounds: Int?, rowSubsample: Double, columnSubsample: Double)

Creates a new set of parameters defining how a boosted tree classifier should be built.

Deprecated


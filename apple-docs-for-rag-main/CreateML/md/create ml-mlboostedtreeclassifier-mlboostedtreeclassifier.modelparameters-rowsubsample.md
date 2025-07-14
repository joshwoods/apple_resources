

- Create ML
- MLBoostedTreeClassifier
- MLBoostedTreeClassifier.ModelParameters
-  rowSubsample 

Instance Property

# rowSubsample

Must be in the range (0, 1).

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 10.14+tvOS 16.0+visionOS 1.0+

``` source
var rowSubsample: Double
```

## See Also

### Accessing parameters

var validationData: MLDataTable?

Validation data represented as a `MLDataTable`.

Deprecated

var maxDepth: Int

var maxIterations: Int

var minLossReduction: Double

var minChildWeight: Double

var randomSeed: Int

var stepSize: Double

Must be in the range (0, 1).

var earlyStoppingRounds: Int?

Validation data must be specified for an early stop.

var columnSubsample: Double

Must be in the range (0, 1).

var validation: MLBoostedTreeClassifier.ModelParameters.ValidationData

Validation data.




- Create ML
- MLBoostedTreeRegressor
- MLBoostedTreeRegressor.ModelParameters
-  earlyStoppingRounds 

Instance Property

# earlyStoppingRounds

Validation data must be specified for an early stop.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 10.14+tvOS 16.0+visionOS 1.0+

``` source
var earlyStoppingRounds: Int?
```

## See Also

### Accessing parameters

var columnSubsample: Double

Must be in the range (0, 1).

var maxDepth: Int

var maxIterations: Int

var minChildWeight: Double

var minLossReduction: Double

var randomSeed: Int

var rowSubsample: Double

Must be in the range (0, 1).

var stepSize: Double

Must be in the range (0, 1).

var validationData: MLDataTable?

Validation data represented as a `MLDataTable`.

Deprecated

var validation: MLBoostedTreeRegressor.ModelParameters.ValidationData

Validation data.


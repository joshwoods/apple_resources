

- Create ML
- MLRandomForestRegressor
- MLRandomForestRegressor.ModelParameters
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

var columnSubsample: Double

Must be in the range (0, 1).

var maxDepth: Int

var maxIterations: Int

var minChildWeight: Double

var minLossReduction: Double

var randomSeed: Int

var validationData: MLDataTable?

Validation data represented as a `MLDataTable`.

Deprecated

var validation: MLRandomForestRegressor.ModelParameters.ValidationData

Validation data.


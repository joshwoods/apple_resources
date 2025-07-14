

- Create ML
- MLBoostedTreeClassifier
- MLBoostedTreeClassifier.ModelParameters
-  validation 

Instance Property

# validation

Validation data.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 10.15+tvOS 16.0+visionOS 1.0+

``` source
var validation: MLBoostedTreeClassifier.ModelParameters.ValidationData { get set }
```

## Discussion

The default is `.split(strategy: .automatic)`, which automatically generates the validation dataset from 0% to 10% of the training dataset.

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

var rowSubsample: Double

Must be in the range (0, 1).

var columnSubsample: Double

Must be in the range (0, 1).


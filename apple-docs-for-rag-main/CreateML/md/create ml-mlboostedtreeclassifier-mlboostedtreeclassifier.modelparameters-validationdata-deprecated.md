

- Create ML
- MLBoostedTreeClassifier
- MLBoostedTreeClassifier.ModelParameters
-  validationData Deprecated

Instance Property

# validationData

Validation data represented as a `MLDataTable`.

iOS 15.0–16.0DeprecatediPadOS 15.0–16.0DeprecatedMac Catalyst 15.0–16.0DeprecatedmacOS 10.14–10.15DeprecatedvisionOS 1.0+

``` source
var validationData: MLDataTable? { get set }
```

Deprecated

Use the validation property instead.

## Discussion

Note

Setting this to `nil` means that the training data will be automatically split for validation. Setting it to an empty table means to not use a validation set.

## See Also

### Accessing parameters

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

var validation: MLBoostedTreeClassifier.ModelParameters.ValidationData

Validation data.


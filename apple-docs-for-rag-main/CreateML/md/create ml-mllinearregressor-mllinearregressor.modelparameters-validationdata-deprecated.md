

- Create ML
- MLLinearRegressor
- MLLinearRegressor.ModelParameters
-  validationData Deprecated

Instance Property

# validationData

Validation data represented as a `MLDataTable`.

iOS 15.0–16.0DeprecatediPadOS 15.0–16.0DeprecatedMac Catalyst 15.0–16.0DeprecatedmacOS 10.14–11.0DeprecatedvisionOS 1.0+

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

var maxIterations: Int

var l1Penalty: Double

var l2Penalty: Double

var stepSize: Double

var convergenceThreshold: Double

var featureRescaling: Bool

var validation: MLLinearRegressor.ModelParameters.ValidationData

Validation data.




- Create ML
- MLDecisionTreeRegressor
- MLDecisionTreeRegressor.ModelParameters
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

var maxDepth: Int

var minChildWeight: Double

var minLossReduction: Double

var randomSeed: Int

var validation: MLDecisionTreeRegressor.ModelParameters.ValidationData

Validation data.


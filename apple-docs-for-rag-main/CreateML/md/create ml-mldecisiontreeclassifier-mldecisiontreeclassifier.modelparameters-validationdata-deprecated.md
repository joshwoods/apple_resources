

- Create ML
- MLDecisionTreeClassifier
- MLDecisionTreeClassifier.ModelParameters
-  validationData Deprecated

Instance Property

# validationData

The data used for the validation set to inform the model training process.

iOS 15.0–16.0DeprecatediPadOS 15.0–16.0DeprecatedMac Catalyst 15.0–16.0DeprecatedmacOS 10.14–10.15DeprecatedvisionOS 1.0+

``` source
var validationData: MLDataTable? { get set }
```

Deprecated

Use the validation property instead.

## See Also

### Accessing parameters

var maxDepth: Int

The maximum depth of the tree. Must be greater than 0.

var minLossReduction: Double

The minimum amount that the loss needs to be reduced to create a new split.

var minChildWeight: Double

The minimum weight of each leaf node.

var randomSeed: Int

The seed value for random operations during tree building process.

var validation: MLDecisionTreeClassifier.ModelParameters.ValidationData

Validation data.


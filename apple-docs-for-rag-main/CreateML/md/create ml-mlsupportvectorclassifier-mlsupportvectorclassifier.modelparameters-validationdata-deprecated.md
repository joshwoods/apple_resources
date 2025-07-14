

- Create ML
- MLSupportVectorClassifier
- MLSupportVectorClassifier.ModelParameters
-  validationData Deprecated

Instance Property

# validationData

Validation data represented as a `MLDataTable`.

macOS 10.14–10.15Deprecated

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

var convergenceThreshold: DoubleDeprecated

var featureRescaling: BoolDeprecated

var maxIterations: IntDeprecated

var penalty: DoubleDeprecated

var validation: MLSupportVectorClassifier.ModelParameters.ValidationData

Validation data.

Deprecated


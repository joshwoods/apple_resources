

- Create ML
- MLSupportVectorClassifier
- MLSupportVectorClassifier.ModelParameters
-  validation Deprecated

Instance Property

# validation

Validation data.

macOS 10.15–14.0Deprecated

``` source
var validation: MLSupportVectorClassifier.ModelParameters.ValidationData { get set }
```

## Discussion

The default is `.split(strategy: .automatic)`, which automatically generates the validation dataset from 0% to 10% of the training dataset.

## See Also

### Accessing parameters

var convergenceThreshold: DoubleDeprecated

var featureRescaling: BoolDeprecated

var maxIterations: IntDeprecated

var penalty: DoubleDeprecated

var validationData: MLDataTable?

Validation data represented as a `MLDataTable`.

Deprecated


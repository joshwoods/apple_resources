

- Create ML
- MLDecisionTreeRegressor
- MLDecisionTreeRegressor.ModelParameters
-  validation 

Instance Property

# validation

Validation data.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 11.0+tvOS 16.0+visionOS 1.0+

``` source
var validation: MLDecisionTreeRegressor.ModelParameters.ValidationData { get set }
```

## Discussion

The default is `.split(strategy: .automatic)`, which automatically generates the validation dataset from 0% to 10% of the training dataset.

## See Also

### Accessing parameters

var maxDepth: Int

var minChildWeight: Double

var minLossReduction: Double

var randomSeed: Int

var validationData: MLDataTable?

Validation data represented as a `MLDataTable`.

Deprecated


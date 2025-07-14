

- Create ML
- MLDecisionTreeClassifier
- MLDecisionTreeClassifier.ModelParameters
-  minLossReduction 

Instance Property

# minLossReduction

The minimum amount that the loss needs to be reduced to create a new split.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 10.14+tvOS 16.0+visionOS 1.0+

``` source
var minLossReduction: Double
```

## See Also

### Accessing parameters

var validationData: MLDataTable?

The data used for the validation set to inform the model training process.

Deprecated

var maxDepth: Int

The maximum depth of the tree. Must be greater than 0.

var minChildWeight: Double

The minimum weight of each leaf node.

var randomSeed: Int

The seed value for random operations during tree building process.

var validation: MLDecisionTreeClassifier.ModelParameters.ValidationData

Validation data.


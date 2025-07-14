

- Create ML
- MLDecisionTreeClassifier
- MLDecisionTreeClassifier.ModelParameters
-  validation 

Instance Property

# validation

Validation data.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 10.15+tvOS 16.0+visionOS 1.0+

``` source
var validation: MLDecisionTreeClassifier.ModelParameters.ValidationData { get set }
```

## Discussion

The default is `.split(strategy: .automatic)`, which automatically generates the validation dataset from 0% to 10% of the training dataset.

## See Also

### Accessing parameters

var validationData: MLDataTable?

The data used for the validation set to inform the model training process.

Deprecated

var maxDepth: Int

The maximum depth of the tree. Must be greater than 0.

var minLossReduction: Double

The minimum amount that the loss needs to be reduced to create a new split.

var minChildWeight: Double

The minimum weight of each leaf node.

var randomSeed: Int

The seed value for random operations during tree building process.


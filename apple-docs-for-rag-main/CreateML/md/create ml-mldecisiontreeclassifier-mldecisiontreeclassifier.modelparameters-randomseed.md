

- Create ML
- MLDecisionTreeClassifier
- MLDecisionTreeClassifier.ModelParameters
-  randomSeed 

Instance Property

# randomSeed

The seed value for random operations during tree building process.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 10.14+tvOS 16.0+visionOS 1.0+

``` source
var randomSeed: Int
```

## Discussion

Set the random seed value to ensure results are reproducible.

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

var validation: MLDecisionTreeClassifier.ModelParameters.ValidationData

Validation data.


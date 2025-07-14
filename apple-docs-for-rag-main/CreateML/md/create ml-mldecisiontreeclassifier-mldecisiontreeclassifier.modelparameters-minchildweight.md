

- Create ML
- MLDecisionTreeClassifier
- MLDecisionTreeClassifier.ModelParameters
-  minChildWeight 

Instance Property

# minChildWeight

The minimum weight of each leaf node.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 10.14+tvOS 16.0+visionOS 1.0+

``` source
var minChildWeight: Double
```

## Discussion

The minimum child weight controls when the tree building should terminate based comparing the sum of the instance weights to the minChildWeight.

## See Also

### Accessing parameters

var validationData: MLDataTable?

The data used for the validation set to inform the model training process.

Deprecated

var maxDepth: Int

The maximum depth of the tree. Must be greater than 0.

var minLossReduction: Double

The minimum amount that the loss needs to be reduced to create a new split.

var randomSeed: Int

The seed value for random operations during tree building process.

var validation: MLDecisionTreeClassifier.ModelParameters.ValidationData

Validation data.


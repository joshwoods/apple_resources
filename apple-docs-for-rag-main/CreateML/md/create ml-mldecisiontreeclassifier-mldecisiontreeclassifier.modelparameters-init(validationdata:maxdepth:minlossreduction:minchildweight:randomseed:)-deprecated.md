

- Create ML
- MLDecisionTreeClassifier
- MLDecisionTreeClassifier.ModelParameters
-  init(validationData:maxDepth:minLossReduction:minChildWeight:randomSeed:) Deprecated

Initializer

# init(validationData:maxDepth:minLossReduction:minChildWeight:randomSeed:)

Creates a new set of parameters.

iOS 15.0–16.0DeprecatediPadOS 15.0–16.0DeprecatedMac Catalyst 15.0–16.0DeprecatedmacOS 10.14–10.15DeprecatedvisionOS 1.0+

``` source
init(
    validationData: MLDataTable?,
    maxDepth: Int = 6,
    minLossReduction: Double = 0,
    minChildWeight: Double = 0.1,
    randomSeed: Int = 42
)
```

Deprecated

Use the validation property instead.

## Parameters 

`validationData`  

The dataset used to monitor how well the model is generalizing.

The default value is `nil` which will use an automatically sampled validation set.

`maxDepth`  

The maximum depth of the tree. Must be a value of at least 1.

The default value is 6.

`minLossReduction`  

The minimum amount of reduction to the loss function that is required to make another node to split the data. Larger values help prevent overfitting.

The default value is 0.

`minChildWeight`  

Determines the minimum weight of each leaf node of the tree. Larger values help prevent overfitting.

The default value is 0.1.

`randomSeed`  

A seed for internal random operations. Set this value to ensure reproducible results.

The default value is 42.

## See Also

### Creating parameters

init(validation: MLDecisionTreeClassifier.ModelParameters.ValidationData, maxDepth: Int, minLossReduction: Double, minChildWeight: Double, randomSeed: Int)

enum ValidationData

Values for specifying validation data.


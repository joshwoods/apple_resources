

- Core ML
- MLParameterKey
-  seed 

Type Property

# seed

The key you use to access the seed parameter that initializes the random number generator for the shuffle option.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.15+tvOS 14.0+visionOS 1.0+watchOS 6.0+

``` source
class var seed: MLParameterKey { get }
```

## Discussion

The value type for the seed key is an Int64.

## See Also

### Accessing Model Update Parameters

class var learningRate: MLParameterKey

The key you use to access the optimizer’s learning rate parameter.

class var momentum: MLParameterKey

The key you use to access the stochastic gradient descent (SGD) optimizer’s momentum parameter.

class var miniBatchSize: MLParameterKey

The key you use to access the optimizer’s mini batch-size parameter.

class var beta1: MLParameterKey

The key you use to access the Adam optimizer’s first beta parameter.

class var beta2: MLParameterKey

The key you use to access the Adam optimizer’s second beta parameter.

class var eps: MLParameterKey

The key you use to access the Adam optimizer’s epsilon parameter.

class var epochs: MLParameterKey

The key you use to access the optimizer’s epochs parameter.

class var shuffle: MLParameterKey

The key you use to access the shuffle parameter, a Boolean value that determines whether the model randomizes the data between epochs.


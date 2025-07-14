

- Core ML
- MLParameterKey
-  biases 

Type Property

# biases

The key you use to access the biases of a layer in a neural network model.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.0+macOS 10.13+tvOS 11.0+visionOS 1.0+watchOS 4.0+

``` source
class var biases: MLParameterKey { get }
```

## Discussion

The value type for the biases key is an MLMultiArray. You must scope this key with the name of the specific neural network layer whose biases you’d like to access. See scoped(to:).

Note

You can only override the biases of a model’s *updatable* layers. Model developers mark these layers as updatable with the Core ML Tools.

## See Also

### Accessing Neural Network Layer Parameters

class var weights: MLParameterKey

The key you use to access the weights of a layer in a neural network model.


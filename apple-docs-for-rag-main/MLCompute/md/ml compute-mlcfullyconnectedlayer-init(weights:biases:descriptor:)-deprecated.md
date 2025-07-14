

- ML Compute
- MLCFullyConnectedLayer
-  init(weights:biases:descriptor:) Deprecated

Initializer

# init(weights:biases:descriptor:)

Creates a fully connected layer with the weights, biases, and convolution descriptor you specify.

iOS 14.0–17.4DeprecatediPadOS 14.0–17.4DeprecatedMac Catalyst 14.0–17.4DeprecatedmacOS 11.0–14.3DeprecatedtvOS 14.0–17.4Deprecated

``` source
convenience init?(
    weights: MLCTensor,
    biases: MLCTensor?,
    descriptor: MLCConvolutionDescriptor
)
```

## Parameters 

`weights`  

The weights tensor.

`biases`  

The biases tensor.

`descriptor`  

An object you use to configure the fully connected layer.

## See Also

### Creating Fully Connected Layers

class MLCConvolutionDescriptor

A configuration object you use to create a convolution or fully connected layer.

Deprecated


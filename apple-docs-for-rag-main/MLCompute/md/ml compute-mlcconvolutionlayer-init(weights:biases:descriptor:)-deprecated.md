

- ML Compute
- MLCConvolutionLayer
-  init(weights:biases:descriptor:) Deprecated

Initializer

# init(weights:biases:descriptor:)

Creates a convolution layer with the weights, biases, and descriptor you specify.

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

The weights tensor.

`descriptor`  

An object you use to configure the multi-head attention layer.

## See Also

### Creating Convolution Layers

class MLCConvolutionDescriptor

A configuration object you use to create a convolution or fully connected layer.

Deprecated


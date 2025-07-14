

- Accelerate
- BNNS
- BNNS.NormalizationLayer
-  init(type:input:output:beta:gamma:momentum:epsilon:activation:filterParameters:) Deprecated

Initializer

# init(type:input:output:beta:gamma:momentum:epsilon:activation:filterParameters:)

Returns a new normalization layer.

iOS 14.0+iPadOS 14.0+Mac CatalystmacOS 11.0+visionOSwatchOS 7.0+tvOS 14.0+

``` source
convenience init?(
    type normalization: BNNS.NormalizationType,
    input: BNNSNDArrayDescriptor,
    output: BNNSNDArrayDescriptor,
    beta: BNNSNDArrayDescriptor,
    gamma: BNNSNDArrayDescriptor,
    momentum: Float = 0,
    epsilon: Float,
    activation: BNNS.ActivationFunction,
    filterParameters: BNNSFilterParameters? = nil
)
```

Deprecated

Use the BNNSGraph API instead.

## Parameters 

`normalization`  

An enumeration that specifies the normalization type.

`input`  

The descriptor of the input.

`output`  

The descriptor of the output.

`beta`  

The descriptor of the beta.

`gamma`  

The descriptor of the gamma.

`momentum`  

A value, between 0 and 1, the normalization operation uses to update the moving mean and moving variance during training.

`epsilon`  

The epsilon in the computation of the standard deviation.

`activation`  

The activation function that the layer applies to the output.

`filterParameters`  

The filter runtime parameters.

## Discussion

Important

The gamma and beta descriptors must match the shape of input up to the normalizaton axis. The input and output descriptors must have a layout of BNNS.DataLayout.imageCHW. The gamma, beta, moving mean, and moving variance descriptors must have a `size[0]` that’s the same as the number of input channels. All arrays must have a data type of `float`.


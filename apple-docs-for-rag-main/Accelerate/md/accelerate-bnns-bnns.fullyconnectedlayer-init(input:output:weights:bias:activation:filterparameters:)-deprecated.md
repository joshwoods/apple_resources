

- Accelerate
- BNNS
- BNNS.FullyConnectedLayer
-  init(input:output:weights:bias:activation:filterParameters:) Deprecated

Initializer

# init(input:output:weights:bias:activation:filterParameters:)

Returns a new fully connected layer.

iOS 14.0+iPadOS 14.0+Mac CatalystmacOS 11.0+visionOSwatchOS 7.0+tvOS 14.0+

``` source
convenience init?(
    input: BNNSNDArrayDescriptor,
    output: BNNSNDArrayDescriptor,
    weights: BNNSNDArrayDescriptor,
    bias: BNNSNDArrayDescriptor?,
    activation: BNNS.ActivationFunction,
    filterParameters: BNNSFilterParameters? = nil
)
```

Deprecated

Use the BNNSGraph API instead.

## Parameters 

`input`  

The descriptor of the input.

`output`  

The descriptor of the output.

`weights`  

The descriptor of the weights.

`bias`  

The descriptor of the bias.

`activation`  

The activation function that the layer applies to the output.

`filterParameters`  

The filter runtime parameters.

## Discussion

Important

The input data type and the weights data type must be equal and be `float`, `float16`, `int8`, or `int16` for the forward pass. The output data type must be `float` for the forward pass. All three arrays must be `float` for the backward pass.


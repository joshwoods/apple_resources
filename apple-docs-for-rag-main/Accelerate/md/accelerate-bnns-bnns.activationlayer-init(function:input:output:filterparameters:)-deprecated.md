

- Accelerate
- BNNS
- BNNS.ActivationLayer
-  init(function:input:output:filterParameters:) Deprecated

Initializer

# init(function:input:output:filterParameters:)

Returns a new activation layer.

iOS 14.0+iPadOS 14.0+Mac CatalystmacOS 11.0+visionOSwatchOS 7.0+tvOS 14.0+

``` source
convenience init?(
    function activationFunction: BNNS.ActivationFunction,
    input: BNNSNDArrayDescriptor,
    output: BNNSNDArrayDescriptor,
    filterParameters: BNNSFilterParameters? = nil
)
```

Deprecated

Use the BNNSGraph API instead.

## Parameters 

`activationFunction`  

The activation function that the layer applies to the output.

`input`  

The descriptor of the input.

`output`  

The descriptor of the output.

`filterParameters`  

The filter runtime parameters.

## Discussion

Important

The input dimensions must be equal to the output dimensions. For activation types other than identity, the input and output must be `float`.


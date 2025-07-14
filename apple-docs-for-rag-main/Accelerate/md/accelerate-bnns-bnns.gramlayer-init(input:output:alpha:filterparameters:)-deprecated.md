

- Accelerate
- BNNS
- BNNS.GramLayer
-  init(input:output:alpha:filterParameters:) Deprecated

Initializer

# init(input:output:alpha:filterParameters:)

Returns a new Gram matrix layer.

iOS 14.0+iPadOS 14.0+Mac CatalystmacOS 11.0+tvOS 14.0+visionOSwatchOS 7.0+

``` source
convenience init?(
    input: BNNSNDArrayDescriptor,
    output: BNNSNDArrayDescriptor,
    alpha: Float,
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

`alpha`  

A value to scale the result.

`filterParameters`  

The filter runtime parameters.


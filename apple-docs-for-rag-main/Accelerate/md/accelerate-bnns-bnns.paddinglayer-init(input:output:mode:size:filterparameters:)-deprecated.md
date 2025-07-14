

- Accelerate
- BNNS
- BNNS.PaddingLayer
-  init(input:output:mode:size:filterParameters:) Deprecated

Initializer

# init(input:output:mode:size:filterParameters:)

Returns a new padding layer.

iOS 14.0+iPadOS 14.0+Mac CatalystmacOS 11.0+visionOSwatchOS 7.0+tvOS 14.0+

``` source
convenience init?(
    input: BNNSNDArrayDescriptor,
    output: BNNSNDArrayDescriptor,
    mode: BNNS.PaddingMode,
    size: [(x: Int, y: Int)],
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

`mode`  

The mode the operation uses to pad.

`size`  

The number of padding elements to add before and after the original data.

`filterParameters`  

The filter runtime parameters.

## Discussion

Important

Padding isn’t supported beyond 4D tensors.


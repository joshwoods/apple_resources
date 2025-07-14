

- Accelerate
- BNNS
- BNNS.DropoutLayer
-  init(input:output:rate:seed:control:filterParameters:) Deprecated

Initializer

# init(input:output:rate:seed:control:filterParameters:)

Returns a new dropout layer.

iOS 14.0+iPadOS 14.0+macOS 11.0+tvOS 14.0+visionOSwatchOS 7.0+Mac Catalyst

``` source
convenience init?(
    input: BNNSNDArrayDescriptor,
    output: BNNSNDArrayDescriptor,
    rate: Float,
    seed: UInt32,
    control: UInt8,
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

`rate`  

The probability that the layer drops out an element or a group of elements.

`seed`  

The seed for the random number generator that the layer ignores if zero.

`control`  

An 8-bit bit mask that indicates the dimension of the grouping of the dropout decision.

`filterParameters`  

The filter runtime parameters.

## Discussion

Important

Dropout layers only support arrays with a data type of `float`. The input shape must be equal to the output shape.


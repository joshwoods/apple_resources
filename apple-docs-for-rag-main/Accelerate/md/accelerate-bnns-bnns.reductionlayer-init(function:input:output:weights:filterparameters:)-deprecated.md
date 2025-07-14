

- Accelerate
- BNNS
- BNNS.ReductionLayer
-  init(function:input:output:weights:filterParameters:) Deprecated

Initializer

# init(function:input:output:weights:filterParameters:)

Returns a new reduction layer.

iOS 14.0+iPadOS 14.0+Mac CatalystmacOS 11.0+tvOS 14.0+watchOS 7.0+visionOS

``` source
convenience init?(
    function reductionFunction: BNNS.ReductionFunction,
    input: BNNSNDArrayDescriptor,
    output: BNNSNDArrayDescriptor,
    weights: BNNSNDArrayDescriptor?,
    filterParameters: BNNSFilterParameters? = nil
)
```

Deprecated

Use the BNNSGraph API instead.

## Parameters 

`reductionFunction`  

The variable that specifies the reduction function.

`input`  

The descriptor of the input.

`output`  

The descriptor of the output.

`weights`  

The descriptor of the weights.

`filterParameters`  

The filter runtime parameters.

## Discussion

Important

The number of input dimensions must be equal to number of output dimensions, and equal to the number of weights dimensions. The reduction layer only supports `float`, with the exception of BNNSReduceFunctionLogicalOr and BNNSReduceFunctionLogicalAnd that support `float` and `BNNSDataTypeBoolean`.


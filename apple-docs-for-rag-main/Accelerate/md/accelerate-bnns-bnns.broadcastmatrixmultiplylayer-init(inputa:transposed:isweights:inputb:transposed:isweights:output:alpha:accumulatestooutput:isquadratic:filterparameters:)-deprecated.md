

- Accelerate
- BNNS
- BNNS.BroadcastMatrixMultiplyLayer
-  init(inputA:transposed:isWeights:inputB:transposed:isWeights:output:alpha:accumulatesToOutput:isQuadratic:filterParameters:) Deprecated

Initializer

# init(inputA:transposed:isWeights:inputB:transposed:isWeights:output:alpha:accumulatesToOutput:isQuadratic:filterParameters:)

Returns a new broadcast matrix multiply layer.

iOS 14.0+iPadOS 14.0+Mac CatalystmacOS 11.0+tvOS 14.0+visionOSwatchOS 7.0+

``` source
convenience init?(
    inputA: BNNSNDArrayDescriptor,
    transposed transposeA: Bool,
    isWeights aIsWeights: Bool,
    inputB: BNNSNDArrayDescriptor,
    transposed transposeB: Bool,
    isWeights bIsWeights: Bool,
    output: BNNSNDArrayDescriptor,
    alpha: Float,
    accumulatesToOutput: Bool,
    isQuadratic: Bool,
    filterParameters: BNNSFilterParameters? = nil
)
```

Deprecated

Use the BNNSGraph API instead.

## Parameters 

`inputA`  

The descriptor of matrix *A*.

`transposeA`  

A Boolean value that transposes the last two dimensions of matrix *A*.

`aIsWeights`  

A Boolean value that determines whether to treat matrix *A* as weights.

`inputB`  

The descriptor of matrix *B*.

`transposeB`  

A Boolean value that transposes the last two dimensions of matrix *B*.

`bIsWeights`  

A Boolean value that determines whether to treat matrix *B* as weights.

`output`  

The descriptor of the output.

`alpha`  

A value to scale the result.

`accumulatesToOutput`  

A Boolean value that specifies whether to add the result to the existing output.

`isQuadratic`  

A Boolean value that determines whether the operation multiplies matrix *A* by itself.

`filterParameters`  

The filter runtime parameters.




- Accelerate
- BNNSLayerParametersReduction
-  init(i_desc:o_desc:w_desc:reduce_func:epsilon:) 

Initializer

# init(i_desc:o_desc:w_desc:reduce_func:epsilon:)

Returns a structure containing the parameters of a reduction layer from the specified parameters.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
init(
    i_desc: BNNSNDArrayDescriptor,
    o_desc: BNNSNDArrayDescriptor,
    w_desc: BNNSNDArrayDescriptor,
    reduce_func: BNNSReduceFunction,
    epsilon: Float
)
```

## Parameters 

`i_desc`  

The descriptor of the input.

`o_desc`  

The descriptor of the output.

`w_desc`  

The descriptor of the weights.

`reduce_func`  

The variable that specifies the reduction function.

`epsilon`  

A value that the operation adds to each element when computing the sum of logarithms.

## Discussion

Important

The number of input dimensions must be equal to number of output dimensions, and equal to the number of weights dimensions. The reduction layer only supports `float`, with the exception of BNNSReduceFunctionLogicalOr and BNNSReduceFunctionLogicalAnd that support `float` and `BNNSDataTypeBoolean`.

## See Also

### Initializers

init()

Returns a structure containing the parameters of a reduction layer.


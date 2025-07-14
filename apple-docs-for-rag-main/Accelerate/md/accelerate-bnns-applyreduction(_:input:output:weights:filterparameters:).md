

- Accelerate
- BNNS
-  applyReduction(\_:input:output:weights:filterParameters:) 

Type Method

# applyReduction(\_:input:output:weights:filterParameters:)

Applies the specified reduction function.

iOS 14.0+iPadOS 14.0+Mac CatalystmacOS 11.0+tvOS 14.0+visionOSwatchOS 7.0+

``` source
static func applyReduction(
    _ reductionFunction: BNNS.ReductionFunction,
    input: BNNSNDArrayDescriptor,
    output: BNNSNDArrayDescriptor,
    weights: BNNSNDArrayDescriptor?,
    filterParameters: BNNSFilterParameters? = nil
) throws
```

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

## See Also

### Reduction layers

class ReductionLayer

A layer object that wraps a reduction filter and manages its deinitialization.

Deprecated

struct BNNSReduceFunction

Constants that describe reduction functions.

struct BNNSLayerParametersReduction

A set of parameters that define a reduction layer.

func BNNSFilterCreateLayerReduction(UnsafePointer&lt;BNNSLayerParametersReduction>, UnsafePointer&lt;BNNSFilterParameters>?) -> BNNSFilter?

Returns a new reduction layer.

Deprecated

func BNNSDirectApplyReduction(UnsafePointer&lt;BNNSLayerParametersReduction>, UnsafePointer&lt;BNNSFilterParameters>?) -> Int32

Applies a reduction operation directly to an input tensor.


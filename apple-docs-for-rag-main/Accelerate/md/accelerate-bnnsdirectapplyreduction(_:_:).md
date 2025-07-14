

- Accelerate
-  BNNSDirectApplyReduction(\_:\_:) 

Function

# BNNSDirectApplyReduction(\_:\_:)

Applies a reduction operation directly to an input tensor.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+watchOS 7.0+

``` source
func BNNSDirectApplyReduction(
    _ layer_params: UnsafePointer,
    _ filter_params: UnsafePointer?
) -> Int32
```

## Parameters 

`layer_params`  

Layer parameters.

`filter_params`  

Filter runtime parameters.

## See Also

### Reduction layers

class ReductionLayer

A layer object that wraps a reduction filter and manages its deinitialization.

Deprecated

static func applyReduction(BNNS.ReductionFunction, input: BNNSNDArrayDescriptor, output: BNNSNDArrayDescriptor, weights: BNNSNDArrayDescriptor?, filterParameters: BNNSFilterParameters?) throws

Applies the specified reduction function.

struct BNNSReduceFunction

Constants that describe reduction functions.

struct BNNSLayerParametersReduction

A set of parameters that define a reduction layer.

func BNNSFilterCreateLayerReduction(UnsafePointer&lt;BNNSLayerParametersReduction>, UnsafePointer&lt;BNNSFilterParameters>?) -> BNNSFilter?

Returns a new reduction layer.

Deprecated


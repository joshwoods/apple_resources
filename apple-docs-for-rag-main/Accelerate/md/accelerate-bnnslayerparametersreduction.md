

- Accelerate
-  BNNSLayerParametersReduction 

Structure

# BNNSLayerParametersReduction

A set of parameters that define a reduction layer.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
struct BNNSLayerParametersReduction
```

## Topics

### Initializers

init(i_desc: BNNSNDArrayDescriptor, o_desc: BNNSNDArrayDescriptor, w_desc: BNNSNDArrayDescriptor, reduce_func: BNNSReduceFunction, epsilon: Float)

Returns a structure containing the parameters of a reduction layer from the specified parameters.

init()

Returns a structure containing the parameters of a reduction layer.

### Instance Properties

var i_desc: BNNSNDArrayDescriptor

The descriptor of the input.

var o_desc: BNNSNDArrayDescriptor

The descriptor of the output.

var w_desc: BNNSNDArrayDescriptor

The descriptor of the weights.

var reduce_func: BNNSReduceFunction

The variable that specifies the reduction function.

var epsilon: Float

A value that the operation adds to each element when computing the sum of logarithms.

## Relationships

### Conforms To

- BitwiseCopyable

## See Also

### Reduction layers

class ReductionLayer

A layer object that wraps a reduction filter and manages its deinitialization.

Deprecated

static func applyReduction(BNNS.ReductionFunction, input: BNNSNDArrayDescriptor, output: BNNSNDArrayDescriptor, weights: BNNSNDArrayDescriptor?, filterParameters: BNNSFilterParameters?) throws

Applies the specified reduction function.

struct BNNSReduceFunction

Constants that describe reduction functions.

func BNNSFilterCreateLayerReduction(UnsafePointer&lt;BNNSLayerParametersReduction>, UnsafePointer&lt;BNNSFilterParameters>?) -> BNNSFilter?

Returns a new reduction layer.

Deprecated

func BNNSDirectApplyReduction(UnsafePointer&lt;BNNSLayerParametersReduction>, UnsafePointer&lt;BNNSFilterParameters>?) -> Int32

Applies a reduction operation directly to an input tensor.


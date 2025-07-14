

- Accelerate
-  BNNSReduceFunction 

Structure

# BNNSReduceFunction

Constants that describe reduction functions.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
struct BNNSReduceFunction
```

## Topics

### Reduction Functions

init(UInt32)

init(rawValue: UInt32)

var rawValue: UInt32

var BNNSReduceFunctionArgMax: BNNSReduceFunction

A reduction function that computes the index of the maximum value.

var BNNSReduceFunctionArgMin: BNNSReduceFunction

A reduction function that computes the index of the minimum value.

var BNNSReduceFunctionL1Norm: BNNSReduceFunction

A reduction function that computes the sum of the absolute value of each element.

var BNNSReduceFunctionLogicalAnd: BNNSReduceFunction

A reduction function that reduces a tensor to true if all elements are true.

var BNNSReduceFunctionAll: BNNSReduceFunction

An alias of the logical AND reduction function.

var BNNSReduceFunctionLogicalOr: BNNSReduceFunction

A reduction function that reduces a tensor to true if any element is true.

var BNNSReduceFunctionLogSum: BNNSReduceFunction

var BNNSReduceFunctionAny: BNNSReduceFunction

An alias of the logical OR reduction function.

var BNNSReduceFunctionMax: BNNSReduceFunction

A reduction function that computes the maximum value.

var BNNSReduceFunctionMean: BNNSReduceFunction

A reduction function that computes the mean value.

var BNNSReduceFunctionMeanNonZero: BNNSReduceFunction

A reduction function that computes the mean value of nonzero elements.

var BNNSReduceFunctionMin: BNNSReduceFunction

A reduction function that computes the minimum value.

var BNNSReduceFunctionSum: BNNSReduceFunction

A reduction function that computes the sum of all values.

var BNNSReduceFunctionSumLog: BNNSReduceFunction

A reduction function that computes the sum of the natural logarithm of all values.

var BNNSReduceFunctionSumSquare: BNNSReduceFunction

A reduction function that computes the sum of the square of all values.

var BNNSReduceFunctionL2Norm: BNNSReduceFunction

A reduction function that computes the Euclidean norm.

var BNNSReduceFunctionLogSumExp: BNNSReduceFunction

A reduction function that computes the logarithm of the sum of the exponentials of each element.

var BNNSReduceFunctionNone: BNNSReduceFunction

A reduction function that copies the input to the output.

var BNNSReduceFunctionProduct: BNNSReduceFunction

A reduction function that computes the product of all values.

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Reduction layers

class ReductionLayer

A layer object that wraps a reduction filter and manages its deinitialization.

Deprecated

static func applyReduction(BNNS.ReductionFunction, input: BNNSNDArrayDescriptor, output: BNNSNDArrayDescriptor, weights: BNNSNDArrayDescriptor?, filterParameters: BNNSFilterParameters?) throws

Applies the specified reduction function.

struct BNNSLayerParametersReduction

A set of parameters that define a reduction layer.

func BNNSFilterCreateLayerReduction(UnsafePointer&lt;BNNSLayerParametersReduction>, UnsafePointer&lt;BNNSFilterParameters>?) -> BNNSFilter?

Returns a new reduction layer.

Deprecated

func BNNSDirectApplyReduction(UnsafePointer&lt;BNNSLayerParametersReduction>, UnsafePointer&lt;BNNSFilterParameters>?) -> Int32

Applies a reduction operation directly to an input tensor.


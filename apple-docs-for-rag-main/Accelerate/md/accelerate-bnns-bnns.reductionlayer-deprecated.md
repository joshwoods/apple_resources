

- Accelerate
- BNNS
-  BNNS.ReductionLayer Deprecated

Class

# BNNS.ReductionLayer

A layer object that wraps a reduction filter and manages its deinitialization.

iOS 14.0+iPadOS 14.0+Mac CatalystmacOS 11.0+visionOSwatchOS 7.0+tvOS 14.0+

``` source
class ReductionLayer
```

Deprecated

Use the BNNSGraph API instead.

## Topics

### Creating a Reduction Layer

convenience init?(function: BNNS.ReductionFunction, input: BNNSNDArrayDescriptor, output: BNNSNDArrayDescriptor, weights: BNNSNDArrayDescriptor?, filterParameters: BNNSFilterParameters?)

Returns a new reduction layer.

### Specifying a Reduction Function

enum ReductionFunction

Constants that describe reduction functions.

### Applying a Reduction Layer

func applyBackward(batchSize: Int, input: BNNSNDArrayDescriptor, output: BNNSNDArrayDescriptor, outputGradient: BNNSNDArrayDescriptor, generatingInputGradient: BNNSNDArrayDescriptor, generatingWeightsGradient: BNNSNDArrayDescriptor?) throws

Applies the layer backward to generate input gradients.

### Directly Applying Reduction

static func applyReduction(BNNS.ReductionFunction, input: BNNSNDArrayDescriptor, output: BNNSNDArrayDescriptor, weights: BNNSNDArrayDescriptor?, filterParameters: BNNSFilterParameters?) throws

Applies the specified reduction function.

## Relationships

### Inherits From

- BNNS.UnaryLayer

## See Also

### Reduction layers

static func applyReduction(BNNS.ReductionFunction, input: BNNSNDArrayDescriptor, output: BNNSNDArrayDescriptor, weights: BNNSNDArrayDescriptor?, filterParameters: BNNSFilterParameters?) throws

Applies the specified reduction function.

struct BNNSReduceFunction

Constants that describe reduction functions.

struct BNNSLayerParametersReduction

A set of parameters that define a reduction layer.

func BNNSFilterCreateLayerReduction(UnsafePointer&lt;BNNSLayerParametersReduction>, UnsafePointer&lt;BNNSFilterParameters>?) -> BNNSFilter?

Returns a new reduction layer.

Deprecated

func BNNSDirectApplyReduction(UnsafePointer&lt;BNNSLayerParametersReduction>, UnsafePointer&lt;BNNSFilterParameters>?) -> Int32

Applies a reduction operation directly to an input tensor.


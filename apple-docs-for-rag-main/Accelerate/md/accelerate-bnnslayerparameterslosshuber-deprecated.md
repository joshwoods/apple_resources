

- Accelerate
-  BNNSLayerParametersLossHuber Deprecated

Structure

# BNNSLayerParametersLossHuber

A structure that contains the parameters of a Huber loss layer.

iOS 14.0–18.0DeprecatediPadOS 14.0–18.0DeprecatedMac Catalyst 14.0–18.0DeprecatedmacOS 11.0–15.0DeprecatedtvOS 14.0–18.0DeprecatedvisionOS 1.0–2.0DeprecatedwatchOS 7.0–11.0Deprecated

``` source
struct BNNSLayerParametersLossHuber
```

Deprecated

Use BNNSGraph\* APIs

## Topics

### Initializers

init(function: BNNSLossFunction, i_desc: BNNSNDArrayDescriptor, o_desc: BNNSNDArrayDescriptor, reduction: BNNSLossReductionFunction, huber_delta: Float)

Returns a new Huber loss layer parameters structure from the specified parameters.

init()

Returns a new Huber loss layer parameters structure.

### Instance Properties

var function: BNNSLossFunction

The function that’s used to compute loss.

var i_desc: BNNSNDArrayDescriptor

The descriptor of the input.

var o_desc: BNNSNDArrayDescriptor

The descriptor of the output.

var reduction: BNNSLossReductionFunction

The function that’s used to reduce the computed loss.

var huber_delta: Float

The boundary value that defines where Huber loss returns mean absolute error or mean square error.

## Relationships

### Conforms To

- BitwiseCopyable

## See Also

### Loss layers

class LossLayer

A layer object that wraps a loss filter and manages its deinitialization.

Deprecated

struct BNNSLossFunction

Constants that describe loss functions.

struct BNNSLossReductionFunction

Constants that describe reduction functions used by a loss layer.

struct BNNSLayerParametersLossBase

A structure that contains the parameters of a loss layer.

Deprecated

struct BNNSLayerParametersLossSigmoidCrossEntropy

A structure that contains the parameters of a sigmoid cross entropy loss layer.

Deprecated

struct BNNSLayerParametersLossSoftmaxCrossEntropy

A structure that contains the parameters of a softmax cross entropy loss layer.

Deprecated

struct BNNSLayerParametersLossYolo

A structure that contains the parameters of a You Only Look Once (YOLO) loss layer.

Deprecated

func BNNSFilterCreateLayerLoss(UnsafeRawPointer, UnsafePointer&lt;BNNSFilterParameters>?) -> BNNSFilter?

Returns a new loss layer.

Deprecated

func BNNSLossFilterApplyBatch(BNNSFilter?, Int, UnsafeRawPointer, Int, UnsafeRawPointer, Int, UnsafeRawPointer?, Int, UnsafeMutableRawPointer, UnsafeMutablePointer&lt;BNNSNDArrayDescriptor>?, Int) -> Int32

Applies a loss filter to a set of input objects, writing the result to a set of output objects.

Deprecated

func BNNSLossFilterApplyBackwardBatch(BNNSFilter?, Int, UnsafeRawPointer, Int, UnsafeMutablePointer&lt;BNNSNDArrayDescriptor>, Int, UnsafeRawPointer, Int, UnsafeRawPointer?, Int, UnsafePointer&lt;BNNSNDArrayDescriptor>, Int) -> Int32

Applies a loss filter backward to generate gradients.

Deprecated


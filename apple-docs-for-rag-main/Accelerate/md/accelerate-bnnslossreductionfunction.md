

- Accelerate
-  BNNSLossReductionFunction 

Structure

# BNNSLossReductionFunction

Constants that describe reduction functions used by a loss layer.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
struct BNNSLossReductionFunction
```

## Topics

### Reduction Functions

var rawValue: UInt32

init(UInt32)

init(rawValue: UInt32)

var BNNSLossReductionMean: BNNSLossReductionFunction

Sums the loss of all samples in the batch and divides by the number of samples.

var BNNSLossReductionNonZeroWeightMean: BNNSLossReductionFunction

Sums the loss of all samples in the batch and divides by the number of non-zero weights.

var BNNSLossReductionSum: BNNSLossReductionFunction

Sums the loss of all samples in the batch.

var BNNSLossReductionWeightedMean: BNNSLossReductionFunction

Sums the loss of all samples in the batch and divides by the sum of all weights.

var BNNSLossReductionNone: BNNSLossReductionFunction

Returns the loss without any reduction.

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Loss layers

class LossLayer

A layer object that wraps a loss filter and manages its deinitialization.

Deprecated

struct BNNSLossFunction

Constants that describe loss functions.

struct BNNSLayerParametersLossBase

A structure that contains the parameters of a loss layer.

Deprecated

struct BNNSLayerParametersLossHuber

A structure that contains the parameters of a Huber loss layer.

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


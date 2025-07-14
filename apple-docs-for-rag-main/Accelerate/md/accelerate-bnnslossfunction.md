

- Accelerate
-  BNNSLossFunction 

Structure

# BNNSLossFunction

Constants that describe loss functions.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
struct BNNSLossFunction
```

## Topics

### Loss Functions

init(UInt32)

init(rawValue: UInt32)

var rawValue: UInt32

var BNNSLossFunctionCategoricalCrossEntropy: BNNSLossFunction

Performs categorical cross entropy computation between input prediction and labels.

var BNNSLossFunctionCosineDistance: BNNSLossFunction

Performs cosine distance loss computation between input predictions and labels.

var BNNSLossFunctionHinge: BNNSLossFunction

Performs Hinge loss computation between labels and unbounded zero-centered binary predictions.

var BNNSLossFunctionHuber: BNNSLossFunction

Huber loss computation between input logits and one-hot encoded labels.

var BNNSLossFunctionLog: BNNSLossFunction

Log loss computation between labels and predictions.

var BNNSLossFunctionMeanAbsoluteError: BNNSLossFunction

Mean absolute error (MAE) computation between input prediction and labels.

var BNNSLossFunctionMeanSquareError: BNNSLossFunction

Mean square error (MSE) computation between input logits and one-hot encoded labels.

var BNNSLossFunctionSigmoidCrossEntropy: BNNSLossFunction

Sigmoid activation on input logits, and independent computation of cross-entropy loss for each class.

var BNNSLossFunctionSoftmaxCrossEntropy: BNNSLossFunction

Softmax activation on input logits, and computation of cross-entropy loss with one-hot encoded labels.

var BNNSLossFunctionYolo: BNNSLossFunction

You Only Look Once (YOLO) loss computation between prediction and ground truth labels.

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

struct BNNSLossReductionFunction

Constants that describe reduction functions used by a loss layer.

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


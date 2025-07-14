

- Accelerate
- BNNS
-  BNNS.LossLayer Deprecated

Class

# BNNS.LossLayer

A layer object that wraps a loss filter and manages its deinitialization.

iOS 14.0+iPadOS 14.0+Mac CatalystmacOS 11.0+tvOS 14.0+watchOS 7.0+visionOS

``` source
class LossLayer
```

Deprecated

Use the BNNSGraph API instead.

## Topics

### Creating a Loss Layer

convenience init?(input: BNNSNDArrayDescriptor, output: BNNSNDArrayDescriptor, lossFunction: BNNS.LossFunction, lossReduction: BNNS.LossReduction, filterParameters: BNNSFilterParameters?)

Returns a new loss layer.

### Specifying a Loss Function

enum LossFunction

Constants that describe loss functions.

### Specifying a Loss Reduction Function

enum LossReduction

An enumeration that describes loss reduction functions.

### Applying a Loss Layer

func apply(batchSize: Int, input: BNNSNDArrayDescriptor, labels: BNNSNDArrayDescriptor, output: BNNSNDArrayDescriptor, generatingInputGradient: BNNSNDArrayDescriptor) throws

Applies the layer to a set of input objects, writing the result to a set of output objects.

### Instance Methods

func apply(batchSize: Int, input: BNNSNDArrayDescriptor, labels: BNNSNDArrayDescriptor, output: BNNSNDArrayDescriptor, weights: BNNSNDArrayDescriptor?, broadcastsWeights: Bool, generatingInputGradient: BNNSNDArrayDescriptor) throws

## Relationships

### Inherits From

- BNNS.Layer

## See Also

### Loss layers

struct BNNSLossFunction

Constants that describe loss functions.

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


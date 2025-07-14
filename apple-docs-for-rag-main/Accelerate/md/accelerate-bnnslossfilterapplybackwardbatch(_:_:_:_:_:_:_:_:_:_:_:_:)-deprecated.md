

- Accelerate
-  BNNSLossFilterApplyBackwardBatch(\_:\_:\_:\_:\_:\_:\_:\_:\_:\_:\_:\_:) Deprecated

Function

# BNNSLossFilterApplyBackwardBatch(\_:\_:\_:\_:\_:\_:\_:\_:\_:\_:\_:\_:)

Applies a loss filter backward to generate gradients.

iOS 14.0–18.0DeprecatediPadOS 14.0–18.0DeprecatedMac Catalyst 14.0–18.0DeprecatedmacOS 11.0–15.0DeprecatedtvOS 14.0–18.0DeprecatedvisionOS 1.0–2.0DeprecatedwatchOS 7.0–11.0Deprecated

``` source
func BNNSLossFilterApplyBackwardBatch(
    _ filter: BNNSFilter?,
    _ batch_size: Int,
    _ in: UnsafeRawPointer,
    _ in_stride: Int,
    _ in_delta: UnsafeMutablePointer,
    _ in_delta_stride: Int,
    _ labels: UnsafeRawPointer,
    _ labels_stride: Int,
    _ weights: UnsafeRawPointer?,
    _ weights_size: Int,
    _ out_delta: UnsafePointer,
    _ out_delta_stride: Int
) -> Int32
```

Deprecated

Use BNNSGraph\* APIs

## Parameters 

`filter`  

The filter to apply.

`batch_size`  

The number of input-output pairs.

`in`  

Pointer to input object.

`in_stride`  

Increment, in values, between input objects.

`in_delta`  

The descriptor of the input delta.

`in_delta_stride`  

Increment, in values, between input delta objects.

`labels`  

Pointer to the labels data.

`labels_stride`  

Increment, in values, between labels.

`weights`  

Pointer to weights delta object.

`weights_size`  

Set to `0` for no weight loss scaling, or `1` for same weight scaling for all samples in the batch.

`out_delta`  

The descriptor of the output delta.

`out_delta_stride`  

Increment, in values, between output delta objects.

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


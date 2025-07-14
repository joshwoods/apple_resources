

- Accelerate
-  BNNSFilterCreateLayerLoss(\_:\_:) Deprecated

Function

# BNNSFilterCreateLayerLoss(\_:\_:)

Returns a new loss layer.

iOS 14.0–18.0DeprecatediPadOS 14.0–18.0DeprecatedMac Catalyst 14.0–18.0DeprecatedmacOS 11.0–15.0DeprecatedtvOS 14.0–18.0DeprecatedvisionOS 1.0–2.0DeprecatedwatchOS 7.0–11.0Deprecated

``` source
func BNNSFilterCreateLayerLoss(
    _ layer_params: UnsafeRawPointer,
    _ filter_params: UnsafePointer?
) -> BNNSFilter?
```

Deprecated

Use BNNSGraph\* APIs

## Parameters 

`layer_params`  

Layer parameters.

`filter_params`  

The filter runtime parameters.

## Discussion

You use a loss layer to compute forward and backward loss.

Forward loss can optionally also compute an optional loss gradient. For example, given the following predicted values in `input`, and ground truth values in `labels`:

```
let input: [Float]  = [9, 1, 6, 3, 4, 5, 6, 7, 8, 9]
let labels: [Float] = [0, 1, 2, 3, 4, 5, 6, 7, 8, 9]
```

The following code computes the loss using BNNSLossFunctionMeanSquareError, reduced to a single value using BNNSLossReductionSum:

```
let n = input.count

var inDelta = [Float](repeating: .nan, count: n)
var output: [Float] = [ .nan ] // expected loss = (9 - 0)² + (6 - 2)² = 97

let flags = BNNSNDArrayFlags(0)

let inputDescriptor = BNNSNDArrayDescriptor(flags: flags,
                                            layout: BNNSDataLayoutVector,
                                            size: (n, 0, 0, 0, 0, 0, 0, 0),
                                            stride: (0, 0, 0, 0, 0, 0, 0, 0),
                                            data: nil,
                                            data_type: .float,
                                            table_data: nil,
                                            table_data_type: .float,
                                            data_scale: 1,
                                            data_bias: 0)

let outputDescriptor = BNNSNDArrayDescriptor(flags: flags,
                                             layout: BNNSDataLayoutVector,
                                             size: (1, 0, 0, 0, 0, 0, 0, 0),
                                             stride: (0, 0, 0, 0, 0, 0, 0, 0),
                                             data: nil,
                                             data_type: .float,
                                             table_data: nil,
                                             table_data_type: .float,
                                             data_scale: 1,
                                             data_bias: 0)

var lossParams = BNNSLayerParametersLossBase(function: BNNSLossFunctionMeanSquareError,
                                             i_desc: inputDescriptor,
                                             o_desc: outputDescriptor,
                                             reduction: BNNSLossReductionSum)

let lossLayer = BNNSFilterCreateLayerLoss(&lossParams, nil)

defer {
    BNNSFilterDestroy(lossLayer)
}

inDelta.withUnsafeMutableBufferPointer { inDeltaPtr in

    var inDeltaDescriptor = BNNSNDArrayDescriptor(flags: flags,
                                                  layout: BNNSDataLayoutVector,
                                                  size: (n, 0, 0, 0, 0, 0, 0, 0),
                                                  stride: (0, 0, 0, 0, 0, 0, 0, 0),
                                                  data: inDeltaPtr.baseAddress,
                                                  data_type: .float,
                                                  table_data: nil,
                                                  table_data_type: .float,
                                                  data_scale: 1,
                                                  data_bias: 0)

    BNNSLossFilterApplyBatch(lossLayer, 1,
                             input, n,
                             labels, n,
                             nil, 0,
                             &output,
                             &inDeltaDescriptor, n)
}
```

On return, `output` contains `(9 - 0)² + (6 - 2)² = 97`, and `inDelta` contains `[18.0, 0.0, 8.0, 0.0, 0.0, 0.0, 0.0, 0.0, 0.0, 0.0]`.

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

func BNNSLossFilterApplyBatch(BNNSFilter?, Int, UnsafeRawPointer, Int, UnsafeRawPointer, Int, UnsafeRawPointer?, Int, UnsafeMutableRawPointer, UnsafeMutablePointer&lt;BNNSNDArrayDescriptor>?, Int) -> Int32

Applies a loss filter to a set of input objects, writing the result to a set of output objects.

Deprecated

func BNNSLossFilterApplyBackwardBatch(BNNSFilter?, Int, UnsafeRawPointer, Int, UnsafeMutablePointer&lt;BNNSNDArrayDescriptor>, Int, UnsafeRawPointer, Int, UnsafeRawPointer?, Int, UnsafePointer&lt;BNNSNDArrayDescriptor>, Int) -> Int32

Applies a loss filter backward to generate gradients.

Deprecated


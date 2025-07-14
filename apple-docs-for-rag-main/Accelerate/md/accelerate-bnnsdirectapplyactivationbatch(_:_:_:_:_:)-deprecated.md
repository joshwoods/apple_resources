

- Accelerate
-  BNNSDirectApplyActivationBatch(\_:\_:\_:\_:\_:) Deprecated

Function

# BNNSDirectApplyActivationBatch(\_:\_:\_:\_:\_:)

Applies an activation filter to a set of input objects, writing out the result to a set of output objects.

iOS 14.0–18.0DeprecatediPadOS 14.0–18.0DeprecatedMac Catalyst 14.0–18.0DeprecatedmacOS 11.0–15.0DeprecatedtvOS 14.0–18.0DeprecatedvisionOS 1.0–2.0DeprecatedwatchOS 7.0–11.0Deprecated

``` source
func BNNSDirectApplyActivationBatch(
    _ layer_params: UnsafePointer,
    _ filter_params: UnsafePointer?,
    _ batch_size: Int,
    _ in_stride: Int,
    _ out_stride: Int
) -> Int32
```

Deprecated

Use BNNSGraph\* APIs

## Parameters 

`layer_params`  

Layer parameters.

`filter_params`  

Filter runtime parameters.

`batch_size`  

The number of input-output pairs.

`in_stride`  

The increment, in values, between inputs.

`out_stride`  

The increment, in values, between outputs.

## Discussion

Calling this function is equal to calling BNNSFilterCreateLayerActivation(_:_:), BNNSFilterApplyBatch(_:_:_:_:_:_:), and BNNSFilterDestroy(_:).

## See Also

### Activation layers

func BNNSFilterCreateVectorActivationLayer(UnsafePointer&lt;BNNSVectorDescriptor>, UnsafePointer&lt;BNNSVectorDescriptor>, UnsafePointer&lt;BNNSActivation>, UnsafePointer&lt;BNNSFilterParameters>?) -> BNNSFilter?Deprecated

class ActivationLayer

A layer object that wraps an activation filter and manages its deinitialization.

Deprecated

struct BNNSActivationFunction

Constants that describe activation functions.

struct BNNSActivation

A set of parameters that describe common activation functions.

struct BNNSLayerParametersActivation

A set of parameters that define an activation layer.

Deprecated

func BNNSFilterCreateLayerActivation(UnsafePointer&lt;BNNSLayerParametersActivation>, UnsafePointer&lt;BNNSFilterParameters>?) -> BNNSFilter?

Returns a new activation layer.

Deprecated

static func applyActivation(activation: BNNS.ActivationFunction, axes: [Int], input: BNNSNDArrayDescriptor, output: BNNSNDArrayDescriptor, batchSize: Int, filterParameters: BNNSFilterParameters?) throws

Applies an activation function on the specified axes.

Deprecated

static func applyActivation(activation: BNNS.ActivationFunction, input: BNNSNDArrayDescriptor, output: BNNSNDArrayDescriptor, batchSize: Int, filterParameters: BNNSFilterParameters?) throws

Applies the specified activation function.

Deprecated


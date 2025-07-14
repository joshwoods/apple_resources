

- Accelerate
-  BNNSFilterCreateVectorActivationLayer(\_:\_:\_:\_:) Deprecated

Function

# BNNSFilterCreateVectorActivationLayer(\_:\_:\_:\_:)

iOS 11.0–14.0DeprecatediPadOS 11.0–14.0DeprecatedMac Catalyst 13.1–14.0DeprecatedmacOS 10.13–11.0DeprecatedtvOS 11.0–14.0DeprecatedvisionOS 1.0–1.0DeprecatedwatchOS 4.0–7.0Deprecated

``` source
func BNNSFilterCreateVectorActivationLayer(
    _ in_desc: UnsafePointer,
    _ out_desc: UnsafePointer,
    _ activation: UnsafePointer,
    _ filter_params: UnsafePointer?
) -> BNNSFilter?
```

Deprecated

Use BNNSFilterCreateLayerActivation(_:_:) instead.

## See Also

### Activation layers

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

func BNNSDirectApplyActivationBatch(UnsafePointer&lt;BNNSLayerParametersActivation>, UnsafePointer&lt;BNNSFilterParameters>?, Int, Int, Int) -> Int32

Applies an activation filter to a set of input objects, writing out the result to a set of output objects.

Deprecated

static func applyActivation(activation: BNNS.ActivationFunction, axes: [Int], input: BNNSNDArrayDescriptor, output: BNNSNDArrayDescriptor, batchSize: Int, filterParameters: BNNSFilterParameters?) throws

Applies an activation function on the specified axes.

Deprecated

static func applyActivation(activation: BNNS.ActivationFunction, input: BNNSNDArrayDescriptor, output: BNNSNDArrayDescriptor, batchSize: Int, filterParameters: BNNSFilterParameters?) throws

Applies the specified activation function.

Deprecated


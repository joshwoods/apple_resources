

- Accelerate
-  BNNSLayerParametersFullyConnected Deprecated

Structure

# BNNSLayerParametersFullyConnected

A structure that contains the parameters of a fully connected layer.

iOS 14.0–18.0DeprecatediPadOS 14.0–18.0DeprecatedMac Catalyst 14.0–18.0DeprecatedmacOS 11.0–15.0DeprecatedtvOS 14.0–18.0DeprecatedvisionOS 1.0–2.0DeprecatedwatchOS 7.0–11.0Deprecated

``` source
struct BNNSLayerParametersFullyConnected
```

Deprecated

Use BNNSGraph\* APIs

## Topics

### Initializers

init(i_desc: BNNSNDArrayDescriptor, w_desc: BNNSNDArrayDescriptor, o_desc: BNNSNDArrayDescriptor, bias: BNNSNDArrayDescriptor, activation: BNNSActivation)

Returns a new fully connected layer parameters structure from the specified parameters.

init()

Returns a new fully connected layer parameters structure.

### Instance Properties

var i_desc: BNNSNDArrayDescriptor

The descriptor of the input.

var w_desc: BNNSNDArrayDescriptor

The descriptor of the weights.

var o_desc: BNNSNDArrayDescriptor

The descriptor of the output.

var bias: BNNSNDArrayDescriptor

The descriptor of the bias.

var activation: BNNSActivation

The activation function that the layer applies to the output.

## Relationships

### Conforms To

- BitwiseCopyable

## See Also

### Fully connected layers

struct BNNSFullyConnectedLayerParameters

A structure containing fully connected layer parameters.

Deprecated

func BNNSFilterCreateFullyConnectedLayer(UnsafePointer&lt;BNNSVectorDescriptor>, UnsafePointer&lt;BNNSVectorDescriptor>, UnsafePointer&lt;BNNSFullyConnectedLayerParameters>, UnsafePointer&lt;BNNSFilterParameters>?) -> BNNSFilter?

Returns a fully connected filter, initialized with input, output, layer, and filter parameters.

Deprecated

class FullyConnectedLayer

A layer object that wraps a fully connected filter and manages its deinitialization.

Deprecated

func BNNSFilterCreateLayerFullyConnected(UnsafePointer&lt;BNNSLayerParametersFullyConnected>, UnsafePointer&lt;BNNSFilterParameters>?) -> BNNSFilter?

Returns a new fully connected layer.

Deprecated


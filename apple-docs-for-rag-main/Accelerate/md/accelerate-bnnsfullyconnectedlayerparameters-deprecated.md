

- Accelerate
-  BNNSFullyConnectedLayerParameters Deprecated

Structure

# BNNSFullyConnectedLayerParameters

A structure containing fully connected layer parameters.

iOS 10.0–14.0DeprecatediPadOS 10.0–14.0DeprecatedMac Catalyst 13.1–14.0DeprecatedmacOS 10.12–11.0DeprecatedtvOS 10.0–14.0DeprecatedvisionOS 1.0–1.0DeprecatedwatchOS 3.0–7.0Deprecated

``` source
struct BNNSFullyConnectedLayerParameters
```

Deprecated

Use BNNSLayerParametersFullyConnected instead.

## Topics

### Initializers

init()

init(in_size: Int, out_size: Int, weights: BNNSLayerData, bias: BNNSLayerData, activation: BNNSActivation)

Returns a new fully connected layer parameters structure.

init(in_size: Int, out_size: Int, weights: BNNSLayerData)

### Instance Properties

var activation: BNNSActivation

The layer activation function.

var bias: BNNSLayerData

Layer bias, one for each output component.

var in_size: Int

The size of the input vector.

var out_size: Int

The size of the output vector.

var weights: BNNSLayerData

Matrix coefficients.

## Relationships

### Conforms To

- BitwiseCopyable

## See Also

### Fully connected layers

func BNNSFilterCreateFullyConnectedLayer(UnsafePointer&lt;BNNSVectorDescriptor>, UnsafePointer&lt;BNNSVectorDescriptor>, UnsafePointer&lt;BNNSFullyConnectedLayerParameters>, UnsafePointer&lt;BNNSFilterParameters>?) -> BNNSFilter?

Returns a fully connected filter, initialized with input, output, layer, and filter parameters.

Deprecated

class FullyConnectedLayer

A layer object that wraps a fully connected filter and manages its deinitialization.

Deprecated

struct BNNSLayerParametersFullyConnected

A structure that contains the parameters of a fully connected layer.

Deprecated

func BNNSFilterCreateLayerFullyConnected(UnsafePointer&lt;BNNSLayerParametersFullyConnected>, UnsafePointer&lt;BNNSFilterParameters>?) -> BNNSFilter?

Returns a new fully connected layer.

Deprecated




- Accelerate
- BNNS
-  BNNS.FullyConnectedLayer Deprecated

Class

# BNNS.FullyConnectedLayer

A layer object that wraps a fully connected filter and manages its deinitialization.

iOS 14.0+iPadOS 14.0+Mac CatalystmacOS 11.0+tvOS 14.0+visionOSwatchOS 7.0+

``` source
class FullyConnectedLayer
```

Deprecated

Use the BNNSGraph API instead.

## Topics

### Creating a Fully Connected Layer

convenience init?(input: BNNSNDArrayDescriptor, output: BNNSNDArrayDescriptor, weights: BNNSNDArrayDescriptor, bias: BNNSNDArrayDescriptor?, activation: BNNS.ActivationFunction, filterParameters: BNNSFilterParameters?)

Returns a new fully connected layer.

### Type Methods

static func sparsify(batchSize: Int, inputLayout: BNNS.SparseLayout, inputDenseShape: BNNSNDArrayDescriptor, inputValues: BNNSNDArrayDescriptor, output: inout BNNSNDArrayDescriptor, sparseParameters: BNNS.SparseParameters?, workspace: UnsafeMutableRawBufferPointer?, filterParameters: BNNSFilterParameters?) throws

Converts a sparse tensor from a standardized sparse layout to a device-specific sparse layout that Fully Connected uses.

## Relationships

### Inherits From

- BNNS.ConvolutionLayer

## See Also

### Fully connected layers

struct BNNSFullyConnectedLayerParameters

A structure containing fully connected layer parameters.

Deprecated

func BNNSFilterCreateFullyConnectedLayer(UnsafePointer&lt;BNNSVectorDescriptor>, UnsafePointer&lt;BNNSVectorDescriptor>, UnsafePointer&lt;BNNSFullyConnectedLayerParameters>, UnsafePointer&lt;BNNSFilterParameters>?) -> BNNSFilter?

Returns a fully connected filter, initialized with input, output, layer, and filter parameters.

Deprecated

struct BNNSLayerParametersFullyConnected

A structure that contains the parameters of a fully connected layer.

Deprecated

func BNNSFilterCreateLayerFullyConnected(UnsafePointer&lt;BNNSLayerParametersFullyConnected>, UnsafePointer&lt;BNNSFilterParameters>?) -> BNNSFilter?

Returns a new fully connected layer.

Deprecated


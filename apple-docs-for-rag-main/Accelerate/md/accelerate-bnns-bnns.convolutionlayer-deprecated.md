

- Accelerate
- BNNS
-  BNNS.ConvolutionLayer Deprecated

Class

# BNNS.ConvolutionLayer

A layer object that wraps a convolution filter and manages its deinitialization.

iOS 14.0+iPadOS 14.0+Mac CatalystmacOS 11.0+tvOS 14.0+visionOSwatchOS 7.0+

``` source
class ConvolutionLayer
```

Deprecated

Use the BNNSGraph API instead.

## Topics

### Creating a Convolution Layer

convenience init?(type: BNNS.ConvolutionType, input: BNNSNDArrayDescriptor, weights: BNNSNDArrayDescriptor, output: BNNSNDArrayDescriptor, bias: BNNSNDArrayDescriptor?, padding: BNNS.ConvolutionPadding, activation: BNNS.ActivationFunction, groupCount: Int, stride: (x: Int, y: Int), dilationStride: (x: Int, y: Int), filterParameters: BNNSFilterParameters?)

Returns a new convolution layer.

### Specifying a Convolution Type

enum ConvolutionType

Constants that describe convolution types.

### Specifying Convolution Padding

enum ConvolutionPadding

Constants that describe convolution padding modes.

### Applying a Convolution Layer

func applyBackward(batchSize: Int, input: BNNSNDArrayDescriptor, output: BNNSNDArrayDescriptor, outputGradient: BNNSNDArrayDescriptor, generatingInputGradient: BNNSNDArrayDescriptor, generatingWeightsGradient: BNNSNDArrayDescriptor?, generatingBiasGradient: BNNSNDArrayDescriptor?) throws

Applies the layer backward to generate input gradients.

## Relationships

### Inherits From

- BNNS.UnaryLayer

### Inherited By

- BNNS.FullyConnectedLayer

## See Also

### Convolution layers

struct BNNSConvolutionLayerParameters

A structure containing convolution parameters.

Deprecated

func BNNSFilterCreateConvolutionLayer(UnsafePointer&lt;BNNSImageStackDescriptor>, UnsafePointer&lt;BNNSImageStackDescriptor>, UnsafePointer&lt;BNNSConvolutionLayerParameters>, UnsafePointer&lt;BNNSFilterParameters>?) -> BNNSFilter?

Returns a convolution filter, initialized with input, output, layer, and filter parameters.

Deprecated

struct BNNSLayerParametersConvolution

A structure that contains the parameters of a convolution layer.

Deprecated

func BNNSFilterCreateLayerConvolution(UnsafePointer&lt;BNNSLayerParametersConvolution>, UnsafePointer&lt;BNNSFilterParameters>?) -> BNNSFilter?

Returns a new convolution layer.

Deprecated

func BNNSFilterCreateLayerTransposedConvolution(UnsafePointer&lt;BNNSLayerParametersConvolution>, UnsafePointer&lt;BNNSFilterParameters>?) -> BNNSFilter?

Returns a new transposed convolution layer.

Deprecated


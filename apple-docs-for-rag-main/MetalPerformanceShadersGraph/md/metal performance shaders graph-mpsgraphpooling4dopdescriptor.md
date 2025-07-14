

- Metal Performance Shaders Graph
-  MPSGraphPooling4DOpDescriptor 

Class

# MPSGraphPooling4DOpDescriptor

The class that defines the parameters for a 4D pooling operation.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+

``` source
class MPSGraphPooling4DOpDescriptor
```

## Overview

Use this descriptor with the following methods:

- maxPooling4D(_:descriptor:name:)

- maxPooling4DReturnIndices(_:descriptor:name:)

- maxPooling4DGradient(_:source:descriptor:name:)

- maxPooling4DGradient(withGradientTensor:indicesTensor:outputShape:descriptor:name:)

- maxPooling4DGradient(withGradientTensor:indicesTensor:outputShapeTensor:descriptor:name:)

- avgPooling4D(_:descriptor:name:)

- avgPooling4DGradient(_:source:descriptor:name:)

- L2NormPooling4D(_:descriptor:name:)

- L2NormPooling4DGradient(_:source:descriptor:name:)

## Topics

### Initializers

convenience init?(kernelSizes: [NSNumber], paddingStyle: MPSGraphPaddingStyle)

Creates a 4D pooling descriptor with default values.

convenience init?(kernelSizes: [NSNumber], strides: [NSNumber], dilationRates: [NSNumber], paddingValues: [NSNumber], paddingStyle: MPSGraphPaddingStyle)

Creates a 4D pooling descriptor with given values.

### Instance Properties

var ceilMode: Bool

Affects how MPSGraph computes the output size: if set to `YES` then output size is computed by rounding up instead of down when dividing input size by stride.

var dilationRates: [NSNumber]

Defines dilation rates for spatial dimensions. Must be four numbers, one for each spatial dimension, fastest running index last.

var includeZeroPadToAverage: Bool

Defines a mode for average pooling, where samples outside the input tensor count as zeroes in the average computation.

var kernelSizes: [NSNumber]

Defines the pooling window size.

var paddingStyle: MPSGraphPaddingStyle

Defines what kind of padding graph applies to the operation.

var paddingValues: [NSNumber]

Defines padding values for spatial dimensions which must be eight numbers, two for each spatial dimension.

var returnIndicesDataType: MPSDataType

Defines the data type for returned indices.

var returnIndicesMode: MPSGraphPoolingReturnIndicesMode

Defines the mode for returned indices of maximum values within each pooling window.

var strides: [NSNumber]

Defines strides for spatial dimensions. Must be four numbers, one for each spatial dimension, fastest running index last.

## Relationships

### Inherits From

- MPSGraphObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCopying
- NSObjectProtocol

## See Also

### Classes

class MPSGraph

The optimized representation of a compute graph of operations and tensors.

class MPSGraphCompilationDescriptor

A class that consists of all the levers for compiling graphs.

class MPSGraphConvolution2DOpDescriptor

A class that describes the properties of a 2D-convolution operator.

class MPSGraphConvolution3DOpDescriptor

A class that describes the properties of a 3D-convolution operator.

class MPSGraphCreateSparseOpDescriptor

A class that describes the properties of a create sparse operation.

class MPSGraphDepthwiseConvolution2DOpDescriptor

A class that defines the parameters for a 2D-depthwise convolution operation.

class MPSGraphDepthwiseConvolution3DOpDescriptor

The class that defines the parameters for a 3D-depthwise convolution operation.

class MPSGraphDevice

A class that describes the compute device.

class MPSGraphExecutable

The compiled representation of a compute graph executable.

class MPSGraphExecutableExecutionDescriptor

A class that consists of all the levers to synchronize and schedule executable execution.

class MPSGraphExecutableSerializationDescriptor

A class that consists of all the levers to serialize an executable.

class MPSGraphExecutionDescriptor

A class that consists of all the levers to synchronize and schedule graph execution.

class MPSGraphFFTDescriptor

The class that defines the parameters for a fast Fourier transform (FFT) operation.

class MPSGraphGRUDescriptor

The class that defines the parameters for a gated recurrent unit (GRU) operation.

class MPSGraphImToColOpDescriptor

The class that defines the parameters for an image to column or column to image operation.


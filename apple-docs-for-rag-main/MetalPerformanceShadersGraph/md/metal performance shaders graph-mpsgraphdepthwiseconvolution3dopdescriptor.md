

- Metal Performance Shaders Graph
-  MPSGraphDepthwiseConvolution3DOpDescriptor 

Class

# MPSGraphDepthwiseConvolution3DOpDescriptor

The class that defines the parameters for a 3D-depthwise convolution operation.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+

``` source
class MPSGraphDepthwiseConvolution3DOpDescriptor
```

## Overview

A `MPSGraphDepthwiseConvolution3DOpDescriptor` defines constant parameters for 3D depthwise convolutions. Use this class with depthwiseConvolution3D(_:weights:descriptor:name:), depthwiseConvolution3DDataGradient(_:weights:outputShape:descriptor:name:) and depthwiseConvolution3DWeightsGradient(_:source:outputShape:descriptor:name:) methods.

## Topics

### Initializers

convenience init?(paddingStyle: MPSGraphPaddingStyle)

Creates a 3D depthwise convolution descriptor with default values.

convenience init?(strides: [NSNumber], dilationRates: [NSNumber], paddingValues: [NSNumber], paddingStyle: MPSGraphPaddingStyle)

Creates a 3D depthwise convolution descriptor with given values.

### Instance Properties

var channelDimensionIndex: Int

The axis that contains the channels in the input and the weights, within the 4D tile of the last dimensions.

var dilationRates: [NSNumber]

The dilation rates for spatial dimensions.

var paddingStyle: MPSGraphPaddingStyle

The padding style for the operation.

var paddingValues: [NSNumber]

The padding values for spatial dimensions.

var strides: [NSNumber]

The strides for spatial dimensions.

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

class MPSGraphLSTMDescriptor

The class that defines the parameters for a long short-term memory (LSTM) operation.


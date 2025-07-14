

- Metal Performance Shaders Graph
-  MPSGraphDepthwiseConvolution2DOpDescriptor 

Class

# MPSGraphDepthwiseConvolution2DOpDescriptor

A class that defines the parameters for a 2D-depthwise convolution operation.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+

``` source
class MPSGraphDepthwiseConvolution2DOpDescriptor
```

## Overview

An `MPSGraphDepthwiseConvolution2DOpDescriptor` defines constant parameters for 2D-depthwise convolutions. Use this class with depthwiseConvolution2D(_:weights:descriptor:name:), depthwiseConvolution2DDataGradient(_:weights:outputShape:descriptor:name:), and depthwiseConvolution2DWeightsGradient(_:source:outputShape:descriptor:name:) methods.

## Topics

### Initializers

convenience init?(dataLayout: MPSGraphTensorNamedDataLayout, weightsLayout: MPSGraphTensorNamedDataLayout)

Creates a 2D-depthwise convolution descriptor with given properties and default values.

convenience init?(strideInX: Int, strideInY: Int, dilationRateInX: Int, dilationRateInY: Int, paddingLeft: Int, paddingRight: Int, paddingTop: Int, paddingBottom: Int, paddingStyle: MPSGraphPaddingStyle, dataLayout: MPSGraphTensorNamedDataLayout, weightsLayout: MPSGraphTensorNamedDataLayout)

Creates a 2D-depthwise convolution descriptor with given values.

### Instance Properties

var dataLayout: MPSGraphTensorNamedDataLayout

The data layout of the input data in the forward pass.

var dilationRateInX: Int

The dilation rate for the x dimension.

var dilationRateInY: Int

The dilation rate for the y dimension.

var paddingBottom: Int

The explicit padding value for the y dimension operation adds after the data.

var paddingLeft: Int

The explicit padding value for the x dimension the operation adds before the data.

var paddingRight: Int

The explicit padding value for the x dimension operation adds after the data.

var paddingStyle: MPSGraphPaddingStyle

The padding style for the operation.

var paddingTop: Int

The explicit padding value for the y dimension operation adds before the data.

var strideInX: Int

The stride for the x dimension.

var strideInY: Int

The stride for the y dimension.

var weightsLayout: MPSGraphTensorNamedDataLayout

The data layout of the weights.

### Instance Methods

func setExplicitPaddingWithPaddingLeft(Int, paddingRight: Int, paddingTop: Int, paddingBottom: Int)

Sets the explicit padding values.

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

class MPSGraphLSTMDescriptor

The class that defines the parameters for a long short-term memory (LSTM) operation.




- Metal Performance Shaders Graph
-  MPSGraphConvolution2DOpDescriptor 

Class

# MPSGraphConvolution2DOpDescriptor

A class that describes the properties of a 2D-convolution operator.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+

``` source
class MPSGraphConvolution2DOpDescriptor
```

## Overview

Use an instance of this class is to add a 2D-convolution operator with the desired properties to the graph.

## Topics

### Initializers

convenience init?(strideInX: Int, strideInY: Int, dilationRateInX: Int, dilationRateInY: Int, groups: Int, paddingLeft: Int, paddingRight: Int, paddingTop: Int, paddingBottom: Int, paddingStyle: MPSGraphPaddingStyle, dataLayout: MPSGraphTensorNamedDataLayout, weightsLayout: MPSGraphTensorNamedDataLayout)

Creates a convolution descriptor with given values for parameters.

convenience init?(strideInX: Int, strideInY: Int, dilationRateInX: Int, dilationRateInY: Int, groups: Int, paddingStyle: MPSGraphPaddingStyle, dataLayout: MPSGraphTensorNamedDataLayout, weightsLayout: MPSGraphTensorNamedDataLayout)

Creates a convolution descriptor with given values for parameters.

### Instance Properties

var dataLayout: MPSGraphTensorNamedDataLayout

The named layout of data in the source tensor.

var dilationRateInX: Int

The amount by which the weights tensor expands in the `x`-direction.

var dilationRateInY: Int

The amount by which the weights tensor expands in the `y`-direction.

var groups: Int

The number of partitions of the input and output channels.

var paddingBottom: Int

The number of zeros added at the bottom of the source tensor.

var paddingLeft: Int

The number of zeros added on the left side of the source tensor.

var paddingRight: Int

The number of zeros added on the right side of the source tensor.

var paddingStyle: MPSGraphPaddingStyle

The type of padding applied to the source tensor.

var paddingTop: Int

The number of zeros added at the top of the source tensor.

var strideInX: Int

The scale that maps `x`-coordinate of the destination to `x`-coordinate of the source.

var strideInY: Int

The scale that maps `y`-coordinate of the destination to `y`-coordinate of the source.

var weightsLayout: MPSGraphTensorNamedDataLayout

The named layout of data in the weights tensor.

### Instance Methods

func setExplicitPaddingWithPaddingLeft(Int, paddingRight: Int, paddingTop: Int, paddingBottom: Int)

Sets the left, right, top, and bottom padding values.

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

class MPSGraphLSTMDescriptor

The class that defines the parameters for a long short-term memory (LSTM) operation.


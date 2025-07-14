

- Metal Performance Shaders Graph
-  MPSGraphConvolution3DOpDescriptor 

Class

# MPSGraphConvolution3DOpDescriptor

A class that describes the properties of a 3D-convolution operator.

iOS 16.3+iPadOS 16.3+Mac Catalyst 16.3+macOS 13.2+tvOS 16.3+visionOS 1.0+

``` source
class MPSGraphConvolution3DOpDescriptor
```

## Overview

Use an instance of this class is to add a 3D-convolution operator with desired properties to the graph.

## Topics

### Initializers

convenience init?(strideInX: Int, strideInY: Int, strideInZ: Int, dilationRateInX: Int, dilationRateInY: Int, dilationRateInZ: Int, groups: Int, paddingLeft: Int, paddingRight: Int, paddingTop: Int, paddingBottom: Int, paddingFront: Int, paddingBack: Int, paddingStyle: MPSGraphPaddingStyle, dataLayout: MPSGraphTensorNamedDataLayout, weightsLayout: MPSGraphTensorNamedDataLayout)

Creates a convolution descriptor with given values for parameters.

convenience init?(strideInX: Int, strideInY: Int, strideInZ: Int, dilationRateInX: Int, dilationRateInY: Int, dilationRateInZ: Int, groups: Int, paddingStyle: MPSGraphPaddingStyle, dataLayout: MPSGraphTensorNamedDataLayout, weightsLayout: MPSGraphTensorNamedDataLayout)

Creates a convolution descriptor with given values for parameters.

### Instance Properties

var dataLayout: MPSGraphTensorNamedDataLayout

The named layout of data in the source tensor.

var dilationRateInX: Int

The amount by which weights tensor expands in the `x`-direction.

var dilationRateInY: Int

The amount by which weights tensor expands in the `y`-direction.

var dilationRateInZ: Int

The amount by which weights tensor expands in the `z`-direction.

var groups: Int

The number of partitions of the input and output channels.

var paddingBack: Int

The number of zeros added at the back of the source tensor.

var paddingBottom: Int

The number of zeros added at the bottom of the source tensor.

var paddingFront: Int

The number of zeros added at the front of the source tensor.

var paddingLeft: Int

The number of zeros added on the left side of the source tensor.

var paddingRight: Int

The number of zeros added on the right side of the source tensor.

var paddingStyle: MPSGraphPaddingStyle

The type of padding that is applied to the source tensor.

var paddingTop: Int

The number of zeros added at the top of the source tensor.

var strideInX: Int

The scale that maps`x`-coordinate of destination to `x`-coordinate of source.

var strideInY: Int

The scale that maps`y`-coordinate of destination to `y`-coordinate of source.

var strideInZ: Int

The scale that maps`z`-coordinate of destination to `z`-coordinate of source.

var weightsLayout: MPSGraphTensorNamedDataLayout

The named layout of data in the weights tensor.

### Instance Methods

func setExplicitPaddingWithPaddingLeft(Int, paddingRight: Int, paddingTop: Int, paddingBottom: Int, paddingFront: Int, paddingBack: Int)

Sets the left, right, top, bottom, front, and back padding values.

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


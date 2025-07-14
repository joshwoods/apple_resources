

- Metal Performance Shaders Graph
-  MPSGraphImToColOpDescriptor 

Class

# MPSGraphImToColOpDescriptor

The class that defines the parameters for an image to column or column to image operation.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+

``` source
class MPSGraphImToColOpDescriptor
```

## Overview

Use this descriptor with the following MPSGraph methods:

- imToCol(_:descriptor:name:)

- colToIm(_:outputShape:descriptor:name:)

## Topics

### Initializers

convenience init?(kernelWidth: Int, kernelHeight: Int, strideInX: Int, strideInY: Int, dilationRateInX: Int, dilationRateInY: Int, dataLayout: MPSGraphTensorNamedDataLayout)

Creates column to image descriptor with given values for parameters.

convenience init?(kernelWidth: Int, kernelHeight: Int, strideInX: Int, strideInY: Int, dilationRateInX: Int, dilationRateInY: Int, paddingLeft: Int, paddingRight: Int, paddingTop: Int, paddingBottom: Int, dataLayout: MPSGraphTensorNamedDataLayout)

Creates an image to column descriptor with given values for parameters.

### Instance Properties

var dataLayout: MPSGraphTensorNamedDataLayout

The property that defines the layout of source or output tensor. e.g. `batch x channels x width x height` for `NCHW` layout

var dilationRateInX: Int

The property that defines the dilation in width dimension.

var dilationRateInY: Int

The property that defines the dilation in height dimension.

var kernelHeight: Int

The property that defines the kernel size in height dimension.

var kernelWidth: Int

The property that defines the kernel size in width dimension.

var paddingBottom: Int

The property that defines the padding in height dimension at the bottom.

var paddingLeft: Int

The property that defines the padding in width dimension on the left side.

var paddingRight: Int

The property that defines the padding in width dimension on the right side.

var paddingTop: Int

The property that defines the padding in height dimension at the top.

var strideInX: Int

The property that defines the stride in width dimension.

var strideInY: Int

The property that defines the stride in height dimension.

### Instance Methods

func setExplicitPaddingWithPaddingLeft(Int, paddingRight: Int, paddingTop: Int, paddingBottom: Int)

Sets the descriptor’s padding to the given values.

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

class MPSGraphLSTMDescriptor

The class that defines the parameters for a long short-term memory (LSTM) operation.


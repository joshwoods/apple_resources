

- Metal Performance Shaders Graph
-  MPSGraphStencilOpDescriptor 

Class

# MPSGraphStencilOpDescriptor

The class that defines the parameters for a stencil operation.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+

``` source
class MPSGraphStencilOpDescriptor
```

## Overview

Use this descriptor with the following MPSGraph method:

- stencil(withSourceTensor:weightsTensor:descriptor:name:)

## Topics

### Initializers

convenience init?(explicitPadding: [NSNumber])

Creates a stencil operation descriptor with default values.

convenience init?(offsets: [NSNumber], explicitPadding: [NSNumber])

Creates a stencil operation descriptor with default values.

convenience init?(paddingStyle: MPSGraphPaddingStyle)

Creates a stencil operation descriptor with default values.

convenience init?(reductionMode: MPSGraphReductionMode, offsets: [NSNumber], strides: [NSNumber], dilationRates: [NSNumber], explicitPadding: [NSNumber], boundaryMode: MPSGraphPaddingMode, paddingStyle: MPSGraphPaddingStyle, paddingConstant: Float)

Creates a stencil operation descriptor with given values.

### Instance Properties

var boundaryMode: MPSGraphPaddingMode

The property that determines which values to use for padding the input tensor.

var dilationRates: [NSNumber]

The property that defines dilation rates for spatial dimensions.

var explicitPadding: [NSNumber]

The property that defines padding values for spatial dimensions.

var offsets: [NSNumber]

An array of length four that determines from which offset to start reading the input tensor.

var paddingConstant: Float

The padding value for `boundaryMode = MPSGraphPaddingModeConstant`.

var paddingStyle: MPSGraphPaddingStyle

The property that defines what kind of padding to apply to the stencil operation.

var reductionMode: MPSGraphReductionMode

The reduction mode to use within the stencil window.

var strides: [NSNumber]

The property that defines strides for spatial dimensions.

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


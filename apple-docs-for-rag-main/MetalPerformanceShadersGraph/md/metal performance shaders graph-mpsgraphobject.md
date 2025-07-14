

- Metal Performance Shaders Graph
-  MPSGraphObject 

Class

# MPSGraphObject

The common base class for all Metal Performance Shaders Graph objects.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+

``` source
class MPSGraphObject
```

## Overview

Only the child classes should be used.

## Relationships

### Inherits From

- NSObject

### Inherited By

- MPSGraph
- MPSGraphCompilationDescriptor
- MPSGraphConvolution2DOpDescriptor
- MPSGraphConvolution3DOpDescriptor
- MPSGraphCreateSparseOpDescriptor
- MPSGraphDepthwiseConvolution2DOpDescriptor
- MPSGraphDepthwiseConvolution3DOpDescriptor
- MPSGraphDevice
- MPSGraphExecutable
- MPSGraphExecutableExecutionDescriptor
- MPSGraphExecutableSerializationDescriptor
- MPSGraphExecutionDescriptor
- MPSGraphFFTDescriptor
- MPSGraphGRUDescriptor
- MPSGraphImToColOpDescriptor
- MPSGraphLSTMDescriptor
- MPSGraphOperation
- MPSGraphPooling2DOpDescriptor
- MPSGraphPooling4DOpDescriptor
- MPSGraphRandomOpDescriptor
- MPSGraphSingleGateRNNDescriptor
- MPSGraphStencilOpDescriptor
- MPSGraphTensor
- MPSGraphTensorData
- MPSGraphType

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
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




- Metal Performance Shaders Graph
-  MPSGraphTensorData 

Class

# MPSGraphTensorData

The representation of a compute data type.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+

``` source
class MPSGraphTensorData
```

## Overview

Pass data to a graph using a tensor data, a reference will be taken to your data and used just in time when the graph is run.

## Topics

### Initializers

init(MPSMatrix)

Initializes a tensor data with an MPS matrix.

init(MPSNDArray)

Initializes an MPSGraphTensorData with an MPS ndarray.

init([MPSImage])

Initializes a tensor data with an MPS image batch.

init(MPSVector)

Initializes a tensor data with an MPS vector.

init(MPSVector, rank: Int)

Initializes a tensor data with an MPS vector enforcing rank of the result.

init(MPSMatrix, rank: Int)

Initializes a tensor data with an MPS matrix enforcing rank of the result.

init(any MTLBuffer, shape: [NSNumber], dataType: MPSDataType)

Initializes an tensor data with a metal buffer.

init(any MTLBuffer, shape: [NSNumber], dataType: MPSDataType, rowBytes: Int)

Initializes an tensor data with a metal buffer.

init(device: MPSGraphDevice, data: Data, shape: [NSNumber], dataType: MPSDataType)

Initializes the tensor data with an `NSData` on a device.

### Instance Properties

var dataType: MPSDataType

The data type of the tensor data.

var device: MPSGraphDevice

The device of the tensor data.

var shape: [NSNumber]

The shape of the tensor data.

### Instance Methods

func mpsndarray() -> MPSNDArray

Return an mpsndarray object will copy contents if the contents are not stored in an MPS ndarray.

## Relationships

### Inherits From

- MPSGraphObject

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


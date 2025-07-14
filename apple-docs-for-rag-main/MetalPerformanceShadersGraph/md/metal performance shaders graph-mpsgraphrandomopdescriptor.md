

- Metal Performance Shaders Graph
-  MPSGraphRandomOpDescriptor 

Class

# MPSGraphRandomOpDescriptor

A class that describes the random operation.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+

``` source
class MPSGraphRandomOpDescriptor
```

## Topics

### Initializers

convenience init?(distribution: MPSGraphRandomDistribution, dataType: MPSDataType)

Class method to initialize a distribution descriptor.

### Instance Properties

var dataType: MPSDataType

The data type of the generated result values.

var distribution: MPSGraphRandomDistribution

The type of distribution to draw samples from. See MPSGraphRandomDistribution.

var max: Float

The upper range of the distribution.

var maxInteger: Int

The upper range of the distribution.

var mean: Float

The mean of the distribution.

var min: Float

The lower range of the distribution.

var minInteger: Int

The lower range of the distribution.

var samplingMethod: MPSGraphRandomNormalSamplingMethod

The sampling method of the distribution.

var standardDeviation: Float

The standard deviation of the distribution.

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


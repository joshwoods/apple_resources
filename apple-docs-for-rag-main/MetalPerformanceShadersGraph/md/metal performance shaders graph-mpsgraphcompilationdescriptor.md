

- Metal Performance Shaders Graph
-  MPSGraphCompilationDescriptor 

Class

# MPSGraphCompilationDescriptor

A class that consists of all the levers for compiling graphs.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+

``` source
class MPSGraphCompilationDescriptor
```

## Topics

### Instance Properties

var callables: [String : MPSGraphExecutable]?

The dictionary used during runtime to lookup the MPSGraphExecutable which correspond to the `symbolName`.

var compilationCompletionHandler: MPSGraphCompilationCompletionHandler

The handler that the graph calls when the compilation completes.

var dispatchQueue: dispatch_queue_t

The dispatch queue used for the compilation.

var optimizationLevel: MPSGraphOptimization

The optimization level for the graph execution, default is MPSGraphOptimizationLevel1.

var optimizationProfile: MPSGraphOptimizationProfile

The optimization profile for the graph optimization.

Deprecated

var waitForCompilationCompletion: Bool

Flag that makes the compile or specialize call blocking till the entire compilation is complete, defaults to NO.

### Instance Methods

func disableTypeInference()

Turns off type inference and relies on type inference during runtime.

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

class MPSGraphLSTMDescriptor

The class that defines the parameters for a long short-term memory (LSTM) operation.


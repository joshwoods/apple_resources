

- Metal Performance Shaders Graph
-  MPSGraphExecutionDescriptor 

Class

# MPSGraphExecutionDescriptor

A class that consists of all the levers to synchronize and schedule graph execution.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+

``` source
class MPSGraphExecutionDescriptor
```

## Topics

### Instance Properties

var compilationDescriptor: MPSGraphCompilationDescriptor?

The compilation descriptor for the graph.

var completionHandler: MPSGraphCompletionHandler

The handler that graph calls at the completion of the execution.

var scheduledHandler: MPSGraphScheduledHandler

The handler that graph calls when it schedules the execution.

var waitUntilCompleted: Bool

The flag that blocks the execution call until the entire execution is complete.

### Instance Methods

func signal(any MTLSharedEvent, atExecutionEvent: MPSGraphExecutionStage, value: UInt64)

Executable signals these shared events at execution stage and immediately proceeds.

func wait(for: any MTLSharedEvent, value: UInt64)

Executable waits on these shared events before scheduling execution on the HW, this does not include encoding which can still continue.

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

class MPSGraphFFTDescriptor

The class that defines the parameters for a fast Fourier transform (FFT) operation.

class MPSGraphGRUDescriptor

The class that defines the parameters for a gated recurrent unit (GRU) operation.

class MPSGraphImToColOpDescriptor

The class that defines the parameters for an image to column or column to image operation.

class MPSGraphLSTMDescriptor

The class that defines the parameters for a long short-term memory (LSTM) operation.


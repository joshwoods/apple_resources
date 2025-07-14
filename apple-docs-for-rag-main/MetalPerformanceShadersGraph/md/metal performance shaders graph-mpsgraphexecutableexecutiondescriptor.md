

- Metal Performance Shaders Graph
-  MPSGraphExecutableExecutionDescriptor 

Class

# MPSGraphExecutableExecutionDescriptor

A class that consists of all the levers to synchronize and schedule executable execution.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+

``` source
class MPSGraphExecutableExecutionDescriptor
```

## Topics

### Instance Properties

var completionHandler: MPSGraphExecutableCompletionHandler

A notification that appears when graph-executable execution is finished.

var scheduledHandler: MPSGraphExecutableScheduledHandler

A notification that appears when graph-executable execution is scheduled.

var waitUntilCompleted: Bool

Flag for the graph executable to wait till the execution has completed.

### Instance Methods

func signal(any MTLSharedEvent, atExecutionEvent: MPSGraphExecutionStage, value: UInt64)

Signals these shared events at execution stage and immediately proceeds.

func wait(for: any MTLSharedEvent, value: UInt64)

Waits on these shared events before scheduling execution on the HW.

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


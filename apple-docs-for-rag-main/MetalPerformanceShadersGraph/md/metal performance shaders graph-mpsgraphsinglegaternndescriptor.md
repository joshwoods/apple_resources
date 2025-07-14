

- Metal Performance Shaders Graph
-  MPSGraphSingleGateRNNDescriptor 

Class

# MPSGraphSingleGateRNNDescriptor

The class that defines the parameters for a single gate RNN operation.

iOS 15.4+iPadOS 15.4+Mac Catalyst 15.4+macOS 12.3+tvOS 15.4+visionOS 1.0+

``` source
class MPSGraphSingleGateRNNDescriptor
```

## Overview

Use this descriptor with the following MPSGraph methods:

- singleGateRNN(_:recurrentWeight:initState:descriptor:name:)

- singleGateRNN(_:recurrentWeight:inputWeight:bias:initState:descriptor:name:)

- singleGateRNN(_:recurrentWeight:inputWeight:bias:initState:mask:descriptor:name:)

- singleGateRNNGradients(_:recurrentWeight:sourceGradient:zState:initState:descriptor:name:)

- singleGateRNNGradients(_:recurrentWeight:sourceGradient:zState:inputWeight:bias:initState:descriptor:name:)

- singleGateRNNGradients(_:recurrentWeight:sourceGradient:zState:inputWeight:bias:initState:mask:descriptor:name:)

- singleGateRNNGradients(_:recurrentWeight:sourceGradient:zState:stateGradient:inputWeight:bias:initState:mask:descriptor:name:)

## Topics

### Instance Properties

var activation: MPSGraphRNNActivation

A parameter that defines the activation function to use with the RNN operation.

var bidirectional: Bool

A parameter that defines a bidirectional RNN layer.

var reverse: Bool

A parameter that defines time direction of the input sequence.

var training: Bool

A parameter that makes the RNN layer support training.

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


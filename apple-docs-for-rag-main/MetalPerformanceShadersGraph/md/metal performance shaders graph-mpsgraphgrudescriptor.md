

- Metal Performance Shaders Graph
-  MPSGraphGRUDescriptor 

Class

# MPSGraphGRUDescriptor

The class that defines the parameters for a gated recurrent unit (GRU) operation.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+

``` source
class MPSGraphGRUDescriptor
```

## Overview

Use this descriptor with the following MPSGraph methods:

- GRU(_:recurrentWeight:inputWeight:bias:descriptor:name:)

- GRU(_:recurrentWeight:inputWeight:bias:initState:descriptor:name:)

- GRU(_:recurrentWeight:inputWeight:bias:initState:mask:secondaryBias:descriptor:name:)

- GRUGradients(_:recurrentWeight:sourceGradient:zState:outputFwd:inputWeight:bias:descriptor:name:)

- GRUGradients(_:recurrentWeight:sourceGradient:zState:outputFwd:inputWeight:bias:initState:descriptor:name:)

- GRUGradients(_:recurrentWeight:sourceGradient:zState:outputFwd:stateGradient:inputWeight:bias:initState:mask:secondaryBias:descriptor:name:)

## Topics

### Instance Properties

var bidirectional: Bool

A parameter that defines a bidirectional GRU layer.

var flipZ: Bool

A parameter that chooses between two variants for the final output computation.

var outputGateActivation: MPSGraphRNNActivation

A parameter that defines the activation function to use with the output-gate of the GRU operation.

var resetAfter: Bool

A parameter that chooses between two variants for the reset gate computation.

var resetGateActivation: MPSGraphRNNActivation

A parameter that defines the activation function to use with the reset-gate of the GRU operation.

var resetGateFirst: Bool

A parameter that controls the internal order of the GRU gates.

var reverse: Bool

A parameter that defines the time direction of the input sequence.

var training: Bool

A parameter that enables the GRU layer to support training.

var updateGateActivation: MPSGraphRNNActivation

A parameter that defines the activation function to use with the update-gate of the GRU operation.

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

class MPSGraphImToColOpDescriptor

The class that defines the parameters for an image to column or column to image operation.

class MPSGraphLSTMDescriptor

The class that defines the parameters for a long short-term memory (LSTM) operation.


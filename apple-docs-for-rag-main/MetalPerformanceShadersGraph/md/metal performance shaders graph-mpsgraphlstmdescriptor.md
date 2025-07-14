

- Metal Performance Shaders Graph
-  MPSGraphLSTMDescriptor 

Class

# MPSGraphLSTMDescriptor

The class that defines the parameters for a long short-term memory (LSTM) operation.

iOS 15.4+iPadOS 15.4+Mac Catalyst 15.4+macOS 12.3+tvOS 15.4+visionOS 1.0+

``` source
class MPSGraphLSTMDescriptor
```

## Overview

Use this descriptor with the following MPSGraph methods:

- LSTM(_:recurrentWeight:initState:initCell:descriptor:name:)

- LSTM(_:recurrentWeight:inputWeight:bias:initState:initCell:descriptor:name:)

- LSTM(_:recurrentWeight:inputWeight:bias:initState:initCell:mask:peephole:descriptor:name:)

- LSTMGradients(_:recurrentWeight:sourceGradient:zState:cellOutputFwd:descriptor:name:)

- LSTMGradients(_:recurrentWeight:sourceGradient:zState:cellOutputFwd:inputWeight:bias:initState:initCell:descriptor:name:)

- LSTMGradients(_:recurrentWeight:sourceGradient:zState:cellOutputFwd:inputWeight:bias:initState:initCell:mask:descriptor:name:)

- LSTMGradients(_:recurrentWeight:sourceGradient:zState:cellOutputFwd:stateGradient:cellGradient:inputWeight:bias:initState:initCell:mask:peephole:descriptor:name:)

## Topics

### Instance Properties

var activation: MPSGraphRNNActivation

A parameter that defines the activation function used with the current cell value of the LSTM operation.

var bidirectional: Bool

A parameter that defines a bidirectional LSTM layer.

var cellGateActivation: MPSGraphRNNActivation

A parameter that defines the activation function used with the cell gate of the LSTM operation.

var forgetGateActivation: MPSGraphRNNActivation

A parameter that defines the activation function used with the forget gate of the LSTM operation.

var forgetGateLast: Bool

A parameter that controls the internal order of the LSTM gates.

var inputGateActivation: MPSGraphRNNActivation

A parameter that defines the activation function used with the input gate of the LSTM operation.

var outputGateActivation: MPSGraphRNNActivation

A parameter that defines the activation function used with the output gate of the LSTM operation.

var produceCell: Bool

A parameter that controls whether or not to return the output cell from the LSTM layer.

var reverse: Bool

A parameter that defines time direction of the input sequence.

var training: Bool

A parameter that enables the LSTM layer to support training.

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


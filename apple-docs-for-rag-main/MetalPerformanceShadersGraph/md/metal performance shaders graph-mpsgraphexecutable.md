

- Metal Performance Shaders Graph
-  MPSGraphExecutable 

Class

# MPSGraphExecutable

The compiled representation of a compute graph executable.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+

``` source
class MPSGraphExecutable
```

## Overview

An `MPSGraphExecutable` is a compiled graph for specific feeds for specific target tensors and target operations.

## Topics

### Initializers

init(coreMLPackageAtURL: URL, descriptor: MPSGraphCompilationDescriptor?)

Initialize the executable with the Core ML model package at the provided URL.

init(package: URL, descriptor: MPSGraphCompilationDescriptor?)

Initialize the executable with the Metal Performance Shaders Graph package at the provided URL.

### Instance Properties

var feedTensors: [MPSGraphTensor]?

Tensors fed to the graph, can be used to order the inputs when executable is created with a graph.

var options: MPSGraphOptions

Options for the graph executable.

var targetTensors: [MPSGraphTensor]?

Tensors targeted by the graph, can be used to order the outputs when executable was created with a graph.

### Instance Methods

func encode(to: MPSCommandBuffer, inputs: [MPSGraphTensorData], results: [MPSGraphTensorData]?, executionDescriptor: MPSGraphExecutableExecutionDescriptor?) -> [MPSGraphTensorData]

Runs the graph for the given feeds and returns the target tensor values, ensuring all target operations also executed. This call is asynchronous and will return immediately after finishing encoding.

func getOutputTypes(with: MPSGraphDevice?, inputTypes: [MPSGraphType], compilationDescriptor: MPSGraphCompilationDescriptor?) -> [MPSGraphShapedType]?

Get output shapes for a specialized executable.

func run(with: any MTLCommandQueue, inputs: [MPSGraphTensorData], results: [MPSGraphTensorData]?, executionDescriptor: MPSGraphExecutableExecutionDescriptor?) -> [MPSGraphTensorData]

Runs the graph for the given feeds and returns the target tensor values, ensuring all target operations also executed.

func runAsync(with: any MTLCommandQueue, inputs: [MPSGraphTensorData], results: [MPSGraphTensorData]?, executionDescriptor: MPSGraphExecutableExecutionDescriptor?) -> [MPSGraphTensorData]

Runs the graph for the given feeds and returns the target tensor values, ensuring all target operations also executed. This call is asynchronous and will return immediately.

func serialize(package: URL, descriptor: MPSGraphExecutableSerializationDescriptor?)

Serialize the MPSGraph executable at the provided url.

func specialize(with: MPSGraphDevice?, inputTypes: [MPSGraphType], compilationDescriptor: MPSGraphCompilationDescriptor?)

Specialize the executable and optimize it.

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


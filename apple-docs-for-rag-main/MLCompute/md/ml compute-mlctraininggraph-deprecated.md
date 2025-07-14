

- ML Compute
-  MLCTrainingGraph Deprecated

Class

# MLCTrainingGraph

A training graph that you create from one or more graph objects plus additional layers you add directly to the training graph.

iOS 14.0–17.4DeprecatediPadOS 14.0–17.4DeprecatedMac Catalyst 14.0–17.4DeprecatedmacOS 11.0–14.3DeprecatedtvOS 14.0–17.4Deprecated

``` source
class MLCTrainingGraph
```

## Overview

The framework provides a family of graph-execution methods to execute a full training iteration, and methods to execute the forward pass, the gradient pass, and optimizer update, individually.

Use one of the `execute` methods to execute a full training iteration to accelerate an ML model represented as a single training graph.

Use one of the `executeForward`, `executeGradient`, or `executeOptimizerUpdatemethods` to accelerate an ML library that separates the forward pass, gradient pass, and optimizer update as separate phases.

## Topics

### Creating Training Graphs

convenience init(graphObjects: [MLCGraph], lossLayer: MLCLayer?, optimizer: MLCOptimizer?)

Creates a training graph with the layers from the graph objects, loss layer, and optimizer you specify.

Optimizers

Create an optimizer to use with the training graph.

class MLCTensorParameter

A tensor parameter object.

### Preparing Training Graphs

func addInputs([String : MLCTensor], lossLabels: [String : MLCTensor]?) -> Bool

Adds the inputs and loss label inputs that you specify to the training graph.

func addInputs([String : MLCTensor], lossLabels: [String : MLCTensor]?, lossLabelWeights: [String : MLCTensor]?) -> Bool

Adds the inputs, loss labels, and loss label weights that you specify to the training graph.

func addOutputs([String : MLCTensor]) -> Bool

Adds the outputs to the training graph you specify.

func stopGradient(for: [MLCTensor]) -> Bool

Adds the tensors that you specify, to indicate which contributions the graph excludes when computing gradients during gradient pass.

func compileOptimizer(MLCOptimizer) -> Bool

Compiles the optimizer to use with a training graph you specify.

func compile(options: MLCGraphCompilationOptions, device: MLCDevice) -> Bool

Compiles the training graph for the options and device you specify.

func compile(options: MLCGraphCompilationOptions, device: MLCDevice, inputTensors: [String : MLCTensor]?, inputTensorsData: [String : MLCTensorData]?) -> Bool

Compiles the training graph for the options, device, and input tensors you specify.

func link(with: [MLCTrainingGraph]) -> Bool

Links the training graphs you specify.

func allocateUserGradient(for: MLCTensor) -> MLCTensor?

Allocates an entry for a gradient for the result tensor you specify.

struct MLCGraphCompilationOptions

A bitmask that specifies the options you use when compiling a graph.

### Executing Training Iterations

func execute(inputsData: [String : MLCTensorData], lossLabelsData: [String : MLCTensorData]?, lossLabelWeightsData: [String : MLCTensorData]?, batchSize: Int, options: MLCExecutionOptions, completionHandler: MLCGraphCompletionHandler?) -> Bool

Executes the training graph with the input data, batch size, execution options, and completion handler you specify.

func execute(inputsData: [String : MLCTensorData], lossLabelsData: [String : MLCTensorData]?, lossLabelWeightsData: [String : MLCTensorData]?, outputsData: [String : MLCTensorData]?, batchSize: Int, options: MLCExecutionOptions, completionHandler: MLCGraphCompletionHandler?) -> Bool

Executes the training graph with the input data, output data, batch size, execution options, and completion handler that you specify.

func synchronizeUpdates()

Synchronizes updates from device memory.

func setTrainingTensorParameters([MLCTensorParameter]) -> Bool

Sets the input tensor parameters, which the optimizer then updates.

struct MLCExecutionOptions

A bitmask that specifies the options you use when executing a graph.

typealias MLCGraphCompletionHandler

A callback completion handler you execute when a graph finishes execution.

### Executing Forward, Gradient, and Optimizer Updates

func executeForward(batchSize: Int, options: MLCExecutionOptions, completionHandler: MLCGraphCompletionHandler?) -> Bool

Executes the forward pass of the training graph with the batch size, execution options, and completion handler you specify.

func executeForward(batchSize: Int, options: MLCExecutionOptions, outputsData: [String : MLCTensorData]?, completionHandler: MLCGraphCompletionHandler?) -> Bool

Executes the forward pass of the training graph with the batch size, execution options, output data, and completion handler you specify.

func executeForward(batchSize: Int, options: MLCExecutionOptions, outputsData: [String : MLCTensorData]?) async throws -> (result: MLCTensor?, executionTime: TimeInterval)

Executes the forward pass of the training graph with the batch size, execution options, and output data you specify.

func executeGradient(batchSize: Int, options: MLCExecutionOptions, completionHandler: MLCGraphCompletionHandler?) -> Bool

Executes the gradient pass of the training graph with the batch size, execution options, and completion handler you specify.

func executeGradient(batchSize: Int, options: MLCExecutionOptions, outputsData: [String : MLCTensorData]?, completionHandler: MLCGraphCompletionHandler?) -> Bool

Executes the gradient pass of the training graph with the batch size, execution options, output data, and completion handler you specify.

func executeGradient(batchSize: Int, options: MLCExecutionOptions, outputsData: [String : MLCTensorData]?) async throws -> TimeInterval

Executes the gradient pass of the training graph with the batch size, execution options, and output data you specify.

func executeOptimizerUpdate(options: MLCExecutionOptions, completionHandler: MLCGraphCompletionHandler?) -> Bool

Executes the optimizer update pass of the training graph with the execution options and completion handler you specify.

func executeOptimizerUpdate(options: MLCExecutionOptions) async throws -> TimeInterval

Executes the optimizer update pass of the training graph with the execution options you specify.

func synchronizeUpdates()

Synchronizes updates from device memory.

func setTrainingTensorParameters([MLCTensorParameter]) -> Bool

Sets the input tensor parameters, which the optimizer then updates.

struct MLCExecutionOptions

A bitmask that specifies the options you use when executing a graph.

typealias MLCGraphCompletionHandler

A callback completion handler you execute when a graph finishes execution.

### Inspecting Training Graphs

func bindOptimizerData([MLCTensorData], deviceData: [MLCTensorOptimizerDeviceData]?, with: MLCTensor) -> Bool

Associates the optimizer and device data you specify along with the tensor.

var optimizer: MLCOptimizer?

The optimizer to use with the training graph.

var deviceMemorySize: Int

The device memory size in bytes for all intermediate tensors for forward, gradient passes, and optimizer updates for all layers in the training graph.

func gradientTensor(forInput: MLCTensor) -> MLCTensor?

Gets the gradient tensor for the input tensor you specify.

func sourceGradientTensors(for: MLCLayer) -> [MLCTensor]

Gets the source gradient tensors for the layer in the training graph you specify.

func resultGradientTensors(for: MLCLayer) -> [MLCTensor]

Gets the result gradient tensors for the layer in the training graph you specify.

func gradientData(forParameter: MLCTensor, layer: MLCLayer) -> Data?

Gets the gradient data for the trainable parameter and associated layer you specify.

## Relationships

### Inherits From

- MLCGraph

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

## See Also

### Graphs

class MLCGraph

A graph of layers you use to build a training or inference graph.

Deprecated

class MLCInferenceGraph

An inference graph created from one or more MLCGraph instances plus additional layers added directly to the inference graph.

Deprecated


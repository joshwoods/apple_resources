

- ML Compute
-  MLCInferenceGraph Deprecated

Class

# MLCInferenceGraph

An inference graph created from one or more MLCGraph instances plus additional layers added directly to the inference graph.

iOS 14.0–17.4DeprecatediPadOS 14.0–17.4DeprecatedMac Catalyst 14.0–17.4DeprecatedmacOS 11.0–14.3DeprecatedtvOS 14.0–17.4Deprecated

``` source
class MLCInferenceGraph
```

## Topics

### Creating Inference Graphs

convenience init(graphObjects: [MLCGraph])

Creates an inference graph with the layers from the graph objects you specify.

### Preparing Inference Graphs

func addInputs([String : MLCTensor]) -> Bool

Adds the inputs you specify to the inference graph.

func addInputs([String : MLCTensor], lossLabels: [String : MLCTensor]?, lossLabelWeights: [String : MLCTensor]?) -> Bool

Adds the inputs, loss labels, and loss label weights that you specify to the inference graph.

func addOutputs([String : MLCTensor]) -> Bool

Adds the outputs you specify to the inference graph.

func compile(options: MLCGraphCompilationOptions, device: MLCDevice) -> Bool

Compiles the inference graph for the options and device you specify.

func compile(options: MLCGraphCompilationOptions, device: MLCDevice, inputTensors: [String : MLCTensor]?, inputTensorsData: [String : MLCTensorData]?) -> Bool

Compiles the inference graph for the options, device, and input tensors you specify.

func link(with: [MLCInferenceGraph]) -> Bool

Links the inference graphs you specify.

struct MLCGraphCompilationOptions

A bitmask that specifies the options you use when compiling a graph.

### Executing Inference Graphs

func execute(inputsData: [String : MLCTensorData], batchSize: Int, options: MLCExecutionOptions, completionHandler: MLCGraphCompletionHandler?) -> Bool

Executes the inference graph with the inputs data, batch size, execution options, and completion handler you specify.

func execute(inputsData: [String : MLCTensorData], outputsData: [String : MLCTensorData]?, batchSize: Int, options: MLCExecutionOptions, completionHandler: MLCGraphCompletionHandler?) -> Bool

Executes the inference graph with the inputs and outputs data, batch size, execution options, and completion handler that you specify.

func execute(inputsData: [String : MLCTensorData], lossLabelsData: [String : MLCTensorData]?, lossLabelWeightsData: [String : MLCTensorData]?, batchSize: Int, options: MLCExecutionOptions, completionHandler: MLCGraphCompletionHandler?) -> Bool

Executes the inference graph with the input data, batch size, execution options and completion handler you specify.

func execute(inputsData: [String : MLCTensorData], lossLabelsData: [String : MLCTensorData]?, lossLabelWeightsData: [String : MLCTensorData]?, outputsData: [String : MLCTensorData]?, batchSize: Int, options: MLCExecutionOptions, completionHandler: MLCGraphCompletionHandler?) -> Bool

Executes the inference graph with the input and output data, batch size, execution options, and completion handler that you specify.

func execute(inputsData: [String : MLCTensorData], lossLabelsData: [String : MLCTensorData]?, lossLabelWeightsData: [String : MLCTensorData]?, outputsData: [String : MLCTensorData]?, batchSize: Int, options: MLCExecutionOptions) async throws -> (result: MLCTensor?, executionTime: TimeInterval)

Executes the inference graph with the input and output data, batch size, and execution options you specify.

struct MLCExecutionOptions

A bitmask that specifies the options you use when executing a graph.

typealias MLCGraphCompletionHandler

A callback completion handler you execute when a graph finishes execution.

### Inspecting Inference Graphs

var deviceMemorySize: Int

The device memory size in bytes for all intermediate tensors in the inference graph.

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

class MLCTrainingGraph

A training graph that you create from one or more graph objects plus additional layers you add directly to the training graph.

Deprecated




- ML Compute
-  MLCExecutionOptions Deprecated

Structure

# MLCExecutionOptions

A bitmask that specifies the options you use when executing a graph.

iOS 14.0–17.4DeprecatediPadOS 14.0–17.4DeprecatedMac Catalyst 14.0–17.4DeprecatedmacOS 11.0–14.3DeprecatedtvOS 14.0–17.4Deprecated

``` source
struct MLCExecutionOptions
```

## Topics

### Execution Options

init(rawValue: UInt64)

Creates an execution option with the specified raw value.

static var skipWritingInputDataToDevice: MLCExecutionOptions

The option to skip writing input data to device memory.

static var synchronous: MLCExecutionOptions

The option to execute the graph synchronously.

static var profiling: MLCExecutionOptions

The option to return profiling information in the callback before returning from execution.

static var perLayerProfiling: MLCExecutionOptions

The option to enable additional per-layer profiling information using signposts.

static var forwardForInference: MLCExecutionOptions

The option to execute the forward pass for inference only.

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- ExpressibleByArrayLiteral
- OptionSet
- RawRepresentable
- Sendable
- SetAlgebra

## See Also

### Executing Inference Graphs

func execute(inputsData: [String : MLCTensorData], batchSize: Int, options: MLCExecutionOptions, completionHandler: MLCGraphCompletionHandler?) -> Bool

Executes the inference graph with the inputs data, batch size, execution options, and completion handler you specify.

Deprecated

func execute(inputsData: [String : MLCTensorData], outputsData: [String : MLCTensorData]?, batchSize: Int, options: MLCExecutionOptions, completionHandler: MLCGraphCompletionHandler?) -> Bool

Executes the inference graph with the inputs and outputs data, batch size, execution options, and completion handler that you specify.

Deprecated

func execute(inputsData: [String : MLCTensorData], lossLabelsData: [String : MLCTensorData]?, lossLabelWeightsData: [String : MLCTensorData]?, batchSize: Int, options: MLCExecutionOptions, completionHandler: MLCGraphCompletionHandler?) -> Bool

Executes the inference graph with the input data, batch size, execution options and completion handler you specify.

Deprecated

func execute(inputsData: [String : MLCTensorData], lossLabelsData: [String : MLCTensorData]?, lossLabelWeightsData: [String : MLCTensorData]?, outputsData: [String : MLCTensorData]?, batchSize: Int, options: MLCExecutionOptions, completionHandler: MLCGraphCompletionHandler?) -> Bool

Executes the inference graph with the input and output data, batch size, execution options, and completion handler that you specify.

Deprecated

func execute(inputsData: [String : MLCTensorData], lossLabelsData: [String : MLCTensorData]?, lossLabelWeightsData: [String : MLCTensorData]?, outputsData: [String : MLCTensorData]?, batchSize: Int, options: MLCExecutionOptions) async throws -> (result: MLCTensor?, executionTime: TimeInterval)

Executes the inference graph with the input and output data, batch size, and execution options you specify.

Deprecated

typealias MLCGraphCompletionHandler

A callback completion handler you execute when a graph finishes execution.


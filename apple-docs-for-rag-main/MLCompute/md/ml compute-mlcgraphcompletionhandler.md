

- ML Compute
-  MLCGraphCompletionHandler 

Type Alias

# MLCGraphCompletionHandler

A callback completion handler you execute when a graph finishes execution.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+

``` source
typealias MLCGraphCompletionHandler = (MLCTensor?, (any Error)?, TimeInterval) -> Void
```

## Parameters 

`resultTensor`  

The result tensor.

`error`  

An error if one occured, otherwise `nil`.

`executionTime`  

The execution time.

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

struct MLCExecutionOptions

A bitmask that specifies the options you use when executing a graph.

Deprecated


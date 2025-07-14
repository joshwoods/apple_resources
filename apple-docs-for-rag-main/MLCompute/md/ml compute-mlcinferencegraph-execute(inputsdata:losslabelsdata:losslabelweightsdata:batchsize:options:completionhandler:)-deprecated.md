

- ML Compute
- MLCInferenceGraph
-  execute(inputsData:lossLabelsData:lossLabelWeightsData:batchSize:options:completionHandler:) Deprecated

Instance Method

# execute(inputsData:lossLabelsData:lossLabelWeightsData:batchSize:options:completionHandler:)

Executes the inference graph with the input data, batch size, execution options and completion handler you specify.

iOS 14.0–17.4DeprecatediPadOS 14.0–17.4DeprecatedMac Catalyst 14.0–17.4DeprecatedmacOS 11.0–14.3DeprecatedtvOS 14.0–17.4Deprecated

``` source
func execute(
    inputsData: [String : MLCTensorData],
    lossLabelsData: [String : MLCTensorData]?,
    lossLabelWeightsData: [String : MLCTensorData]?,
    batchSize: Int,
    options: MLCExecutionOptions = [],
    completionHandler: MLCGraphCompletionHandler? = nil
) -> Bool
```

## Parameters 

`inputsData`  

A dictionary that contains input data.

`lossLabelsData`  

A dictionary that contains loss label data.

`lossLabelWeightsData`  

A dictionary that contains loss label weight data.

`batchSize`  

The batch size.

`options`  

The execution options.

`completionHandler`  

The completion handler.

## Return Value

`true` if the execution was successful.

## Discussion

When executing an inference graph, if an optimizer is specified, the optimizer update is applied.

For variable length sequences for LSTMs/RNNs, use the key `“sortedSequenceLengths”` and pass in tensor data created by using one of the MLCTensor sequence length initializers as the value.

If synchronous is specified in `options`, this method returns after the graph is executed. Otherwise, this method returns after the graph is queued for execution. The completion handler is called after the graph has finished execution.

## See Also

### Executing Inference Graphs

func execute(inputsData: [String : MLCTensorData], batchSize: Int, options: MLCExecutionOptions, completionHandler: MLCGraphCompletionHandler?) -> Bool

Executes the inference graph with the inputs data, batch size, execution options, and completion handler you specify.

Deprecated

func execute(inputsData: [String : MLCTensorData], outputsData: [String : MLCTensorData]?, batchSize: Int, options: MLCExecutionOptions, completionHandler: MLCGraphCompletionHandler?) -> Bool

Executes the inference graph with the inputs and outputs data, batch size, execution options, and completion handler that you specify.

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

typealias MLCGraphCompletionHandler

A callback completion handler you execute when a graph finishes execution.


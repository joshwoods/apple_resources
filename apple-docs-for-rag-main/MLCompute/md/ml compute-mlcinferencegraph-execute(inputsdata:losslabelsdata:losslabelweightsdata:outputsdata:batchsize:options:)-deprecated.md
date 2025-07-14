

- ML Compute
- MLCInferenceGraph
-  execute(inputsData:lossLabelsData:lossLabelWeightsData:outputsData:batchSize:options:) Deprecated

Instance Method

# execute(inputsData:lossLabelsData:lossLabelWeightsData:outputsData:batchSize:options:)

Executes the inference graph with the input and output data, batch size, and execution options you specify.

iOS 15.0–17.0DeprecatediPadOS 15.0–17.0DeprecatedMac Catalyst 15.0–17.0DeprecatedmacOS 12.0–14.0DeprecatedtvOS 15.0–17.0Deprecated

``` source
@discardableResult
func execute(
    inputsData: [String : MLCTensorData],
    lossLabelsData: [String : MLCTensorData]? = nil,
    lossLabelWeightsData: [String : MLCTensorData]? = nil,
    outputsData: [String : MLCTensorData]? = nil,
    batchSize: Int,
    options: MLCExecutionOptions = []
) async throws -> (result: MLCTensor?, executionTime: TimeInterval)
```

Deprecated

Use Metal Performance Shaders Graph or BNNS instead.

## Parameters 

`inputsData`  

A dictionary that contains input data.

`lossLabelsData`  

A dictionary that contains loss label data.

`lossLabelWeightsData`  

A dictionary that contains loss label weight data.

`outputsData`  

A dictionary that contains output data.

`batchSize`  

The batch size.

`options`  

The execution options.

## Return Value

The result tensor, if any, and the execution time if you specify profiling.

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

struct MLCExecutionOptions

A bitmask that specifies the options you use when executing a graph.

Deprecated

typealias MLCGraphCompletionHandler

A callback completion handler you execute when a graph finishes execution.


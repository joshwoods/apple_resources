

- ML Compute
- MLCTrainingGraph
-  execute(inputsData:lossLabelsData:lossLabelWeightsData:batchSize:options:completionHandler:) Deprecated

Instance Method

# execute(inputsData:lossLabelsData:lossLabelWeightsData:batchSize:options:completionHandler:)

Executes the training graph with the input data, batch size, execution options, and completion handler you specify.

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

A dictionary that contains loss labels data.

`lossLabelWeightsData`  

A dictionary that contains loss label weights data.

`batchSize`  

The batch size.

`options`  

The execution options.

`completionHandler`  

The completion handler.

## Return Value

`true` if the execution was successful.

## Discussion

When you execute a training iteration, if you specified an optimizer when you created the graph, the framework applies the optimizer update.

For variable length sequences for LSTMs/RNNs, use the key “`sortedSequenceLength`” and pass in tensor data created by using one of the MLCTensor sequence length initializers as the value.

If you include synchronous in `options`, the execution method only returns after the graph has finished execution. Otherwise, the execution method returns once the framework enqueues the graph for execution. However, the completion handler is still not called until after the graph has finished execution.

## See Also

### Executing Training Iterations

func execute(inputsData: [String : MLCTensorData], lossLabelsData: [String : MLCTensorData]?, lossLabelWeightsData: [String : MLCTensorData]?, outputsData: [String : MLCTensorData]?, batchSize: Int, options: MLCExecutionOptions, completionHandler: MLCGraphCompletionHandler?) -> Bool

Executes the training graph with the input data, output data, batch size, execution options, and completion handler that you specify.

Deprecated

func synchronizeUpdates()

Synchronizes updates from device memory.

Deprecated

func setTrainingTensorParameters([MLCTensorParameter]) -> Bool

Sets the input tensor parameters, which the optimizer then updates.

Deprecated

struct MLCExecutionOptions

A bitmask that specifies the options you use when executing a graph.

Deprecated

typealias MLCGraphCompletionHandler

A callback completion handler you execute when a graph finishes execution.


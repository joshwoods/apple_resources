

- ML Compute
- MLCTrainingGraph
-  synchronizeUpdates() Deprecated

Instance Method

# synchronizeUpdates()

Synchronizes updates from device memory.

iOS 14.0–17.4DeprecatediPadOS 14.0–17.4DeprecatedMac Catalyst 14.0–17.4DeprecatedmacOS 11.0–14.3DeprecatedtvOS 14.0–17.4Deprecated

``` source
func synchronizeUpdates()
```

## Discussion

This method synchronizes the weights/biases from convolution, fully connected and LSTM layers, and tensor parameters, from device memory to host memory.

## See Also

### Executing Training Iterations

func execute(inputsData: [String : MLCTensorData], lossLabelsData: [String : MLCTensorData]?, lossLabelWeightsData: [String : MLCTensorData]?, batchSize: Int, options: MLCExecutionOptions, completionHandler: MLCGraphCompletionHandler?) -> Bool

Executes the training graph with the input data, batch size, execution options, and completion handler you specify.

Deprecated

func execute(inputsData: [String : MLCTensorData], lossLabelsData: [String : MLCTensorData]?, lossLabelWeightsData: [String : MLCTensorData]?, outputsData: [String : MLCTensorData]?, batchSize: Int, options: MLCExecutionOptions, completionHandler: MLCGraphCompletionHandler?) -> Bool

Executes the training graph with the input data, output data, batch size, execution options, and completion handler that you specify.

Deprecated

func setTrainingTensorParameters([MLCTensorParameter]) -> Bool

Sets the input tensor parameters, which the optimizer then updates.

Deprecated

struct MLCExecutionOptions

A bitmask that specifies the options you use when executing a graph.

Deprecated

typealias MLCGraphCompletionHandler

A callback completion handler you execute when a graph finishes execution.


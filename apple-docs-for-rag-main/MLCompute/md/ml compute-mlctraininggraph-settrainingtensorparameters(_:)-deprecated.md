

- ML Compute
- MLCTrainingGraph
-  setTrainingTensorParameters(\_:) Deprecated

Instance Method

# setTrainingTensorParameters(\_:)

Sets the input tensor parameters, which the optimizer then updates.

iOS 14.0–17.4DeprecatediPadOS 14.0–17.4DeprecatedMac Catalyst 14.0–17.4DeprecatedmacOS 11.0–14.3DeprecatedtvOS 14.0–17.4Deprecated

``` source
func setTrainingTensorParameters(_ parameters: [MLCTensorParameter]) -> Bool
```

## Parameters 

`parameters`  

An array that contains the input tensor parameters.

## Return Value

`true` if the operation was successful.

## See Also

### Executing Training Iterations

func execute(inputsData: [String : MLCTensorData], lossLabelsData: [String : MLCTensorData]?, lossLabelWeightsData: [String : MLCTensorData]?, batchSize: Int, options: MLCExecutionOptions, completionHandler: MLCGraphCompletionHandler?) -> Bool

Executes the training graph with the input data, batch size, execution options, and completion handler you specify.

Deprecated

func execute(inputsData: [String : MLCTensorData], lossLabelsData: [String : MLCTensorData]?, lossLabelWeightsData: [String : MLCTensorData]?, outputsData: [String : MLCTensorData]?, batchSize: Int, options: MLCExecutionOptions, completionHandler: MLCGraphCompletionHandler?) -> Bool

Executes the training graph with the input data, output data, batch size, execution options, and completion handler that you specify.

Deprecated

func synchronizeUpdates()

Synchronizes updates from device memory.

Deprecated

struct MLCExecutionOptions

A bitmask that specifies the options you use when executing a graph.

Deprecated

typealias MLCGraphCompletionHandler

A callback completion handler you execute when a graph finishes execution.


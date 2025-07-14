

- ML Compute
- MLCTrainingGraph
-  executeGradient(batchSize:options:outputsData:) Deprecated

Instance Method

# executeGradient(batchSize:options:outputsData:)

Executes the gradient pass of the training graph with the batch size, execution options, and output data you specify.

iOS 15.0–17.0DeprecatediPadOS 15.0–17.0DeprecatedMac Catalyst 15.0–17.0DeprecatedmacOS 12.0–14.0DeprecatedtvOS 15.0–17.0Deprecated

``` source
@discardableResult
func executeGradient(
    batchSize: Int,
    options: MLCExecutionOptions = [],
    outputsData: [String : MLCTensorData]? = nil
) async throws -> TimeInterval
```

Deprecated

Use Metal Performance Shaders Graph or BNNS instead.

## Parameters 

`batchSize`  

The batch size.

`options`  

The execution options.

`outputsData`  

A dictionary that contains output data.

## Return Value

The execution time if you specify profiling.

## See Also

### Executing Forward, Gradient, and Optimizer Updates

func executeForward(batchSize: Int, options: MLCExecutionOptions, completionHandler: MLCGraphCompletionHandler?) -> Bool

Executes the forward pass of the training graph with the batch size, execution options, and completion handler you specify.

Deprecated

func executeForward(batchSize: Int, options: MLCExecutionOptions, outputsData: [String : MLCTensorData]?, completionHandler: MLCGraphCompletionHandler?) -> Bool

Executes the forward pass of the training graph with the batch size, execution options, output data, and completion handler you specify.

Deprecated

func executeForward(batchSize: Int, options: MLCExecutionOptions, outputsData: [String : MLCTensorData]?) async throws -> (result: MLCTensor?, executionTime: TimeInterval)

Executes the forward pass of the training graph with the batch size, execution options, and output data you specify.

Deprecated

func executeGradient(batchSize: Int, options: MLCExecutionOptions, completionHandler: MLCGraphCompletionHandler?) -> Bool

Executes the gradient pass of the training graph with the batch size, execution options, and completion handler you specify.

Deprecated

func executeGradient(batchSize: Int, options: MLCExecutionOptions, outputsData: [String : MLCTensorData]?, completionHandler: MLCGraphCompletionHandler?) -> Bool

Executes the gradient pass of the training graph with the batch size, execution options, output data, and completion handler you specify.

Deprecated

func executeOptimizerUpdate(options: MLCExecutionOptions, completionHandler: MLCGraphCompletionHandler?) -> Bool

Executes the optimizer update pass of the training graph with the execution options and completion handler you specify.

Deprecated

func executeOptimizerUpdate(options: MLCExecutionOptions) async throws -> TimeInterval

Executes the optimizer update pass of the training graph with the execution options you specify.

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


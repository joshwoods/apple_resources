

- ML Compute
- MLCExecutionOptions
-  forwardForInference Deprecated

Type Property

# forwardForInference

The option to execute the forward pass for inference only.

iOS 14.0–17.4DeprecatediPadOS 14.0–17.4DeprecatedMac Catalyst 14.0–17.4DeprecatedmacOS 11.0–14.3DeprecatedtvOS 14.0–17.4Deprecated

``` source
static var forwardForInference: MLCExecutionOptions { get }
```

## Discussion

If you include this option and execute a training graph using one of the `execute` methods, such as execute(inputsData:lossLabelsData:lossLabelWeightsData:batchSize:options:completionHandler:), the framework only executes the forward pass of the training graph, and it executes that forward pass for inference only.

If you include this option and execute a training graph using one of the `executeForward` methods, such as executeForward(batchSize:options:completionHandler:), the framework executes the forward pass for inference only.

## See Also

### Execution Options

init(rawValue: UInt64)

Creates an execution option with the specified raw value.

Deprecated

static var skipWritingInputDataToDevice: MLCExecutionOptions

The option to skip writing input data to device memory.

Deprecated

static var synchronous: MLCExecutionOptions

The option to execute the graph synchronously.

Deprecated

static var profiling: MLCExecutionOptions

The option to return profiling information in the callback before returning from execution.

Deprecated

static var perLayerProfiling: MLCExecutionOptions

The option to enable additional per-layer profiling information using signposts.

Deprecated


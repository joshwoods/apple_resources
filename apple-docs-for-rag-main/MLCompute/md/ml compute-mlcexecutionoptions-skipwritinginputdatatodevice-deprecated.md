

- ML Compute
- MLCExecutionOptions
-  skipWritingInputDataToDevice Deprecated

Type Property

# skipWritingInputDataToDevice

The option to skip writing input data to device memory.

iOS 14.0–17.4DeprecatediPadOS 14.0–17.4DeprecatedMac Catalyst 14.0–17.4DeprecatedmacOS 11.0–14.3DeprecatedtvOS 14.0–17.4Deprecated

``` source
static var skipWritingInputDataToDevice: MLCExecutionOptions { get }
```

## Discussion

Include this option to prevent writing the input tensors to device memory associated with these tensors when the framework executes the graph.

## See Also

### Execution Options

init(rawValue: UInt64)

Creates an execution option with the specified raw value.

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

static var forwardForInference: MLCExecutionOptions

The option to execute the forward pass for inference only.

Deprecated


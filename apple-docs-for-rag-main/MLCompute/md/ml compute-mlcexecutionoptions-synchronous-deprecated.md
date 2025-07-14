

- ML Compute
- MLCExecutionOptions
-  synchronous Deprecated

Type Property

# synchronous

The option to execute the graph synchronously.

iOS 14.0–17.4DeprecatediPadOS 14.0–17.4DeprecatedMac Catalyst 14.0–17.4DeprecatedmacOS 11.0–14.3DeprecatedtvOS 14.0–17.4Deprecated

``` source
static var synchronous: MLCExecutionOptions { get }
```

## Discussion

Include this option to wait until execution of the graph on specified device finishes before returning from the execute method.

## See Also

### Execution Options

init(rawValue: UInt64)

Creates an execution option with the specified raw value.

Deprecated

static var skipWritingInputDataToDevice: MLCExecutionOptions

The option to skip writing input data to device memory.

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


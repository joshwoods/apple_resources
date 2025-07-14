

- ML Compute
- MLCExecutionOptions
-  perLayerProfiling Deprecated

Type Property

# perLayerProfiling

The option to enable additional per-layer profiling information using signposts.

iOS 15.0–17.4DeprecatediPadOS 15.0–17.4DeprecatedMac Catalyst 15.0–17.4DeprecatedmacOS 12.0–14.3DeprecatedtvOS 15.0–17.4Deprecated

``` source
static var perLayerProfiling: MLCExecutionOptions { get }
```

## Discussion

Visualize the layer information using the Logging profiling template in Instruments. This information may not be available for all ML Compute devices.

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

static var forwardForInference: MLCExecutionOptions

The option to execute the forward pass for inference only.

Deprecated


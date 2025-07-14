

- ML Compute
- MLCGraphCompilationOptions
-  debugLayers Deprecated

Type Property

# debugLayers

The option to debug layers during graph compilation.

iOS 14.0–17.4DeprecatediPadOS 14.0–17.4DeprecatedMac Catalyst 14.0–17.4DeprecatedmacOS 11.0–14.3DeprecatedtvOS 14.0–17.4Deprecated

``` source
static var debugLayers: MLCGraphCompilationOptions { get }
```

## Discussion

Include this option to disable various optimizations such as layer fusion, and ensure the framework synchronizes the resulting forward and gradients tensors host memory with device memory, for layers marked as debuggable.

## See Also

### Creating Graph Compilation Options

init(rawValue: UInt64)

Creates a graph compilation option with the specified raw value.

Deprecated

static var disableLayerFusion: MLCGraphCompilationOptions

The option to disable layer fusion during graph compilation.

Deprecated

static var linkGraphs: MLCGraphCompilationOptions

The option to link graphs during graph compilation.

Deprecated

static var computeAllGradients: MLCGraphCompilationOptions

The option to compute all gradients during graph compilation.

Deprecated


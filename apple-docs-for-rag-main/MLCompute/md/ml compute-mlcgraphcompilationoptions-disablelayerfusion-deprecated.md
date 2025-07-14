

- ML Compute
- MLCGraphCompilationOptions
-  disableLayerFusion Deprecated

Type Property

# disableLayerFusion

The option to disable layer fusion during graph compilation.

iOS 14.0–17.4DeprecatediPadOS 14.0–17.4DeprecatedMac Catalyst 14.0–17.4DeprecatedmacOS 11.0–14.3DeprecatedtvOS 14.0–17.4Deprecated

``` source
static var disableLayerFusion: MLCGraphCompilationOptions { get }
```

## Discussion

Include this option to disable fusion of layers, which is an important optimization that helps performance and memory footprint.

## See Also

### Creating Graph Compilation Options

init(rawValue: UInt64)

Creates a graph compilation option with the specified raw value.

Deprecated

static var debugLayers: MLCGraphCompilationOptions

The option to debug layers during graph compilation.

Deprecated

static var linkGraphs: MLCGraphCompilationOptions

The option to link graphs during graph compilation.

Deprecated

static var computeAllGradients: MLCGraphCompilationOptions

The option to compute all gradients during graph compilation.

Deprecated


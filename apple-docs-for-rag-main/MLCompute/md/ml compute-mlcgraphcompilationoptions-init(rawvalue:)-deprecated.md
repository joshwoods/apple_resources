

- ML Compute
- MLCGraphCompilationOptions
-  init(rawValue:) Deprecated

Initializer

# init(rawValue:)

Creates a graph compilation option with the specified raw value.

iOS 14.0–17.4DeprecatediPadOS 14.0–17.4DeprecatedMac Catalyst 14.0–17.4DeprecatedmacOS 11.0–14.3DeprecatedtvOS 14.0–17.4Deprecated

``` source
init(rawValue: UInt64)
```

## Parameters 

`rawValue`  

The bitmask raw value.

## See Also

### Creating Graph Compilation Options

static var debugLayers: MLCGraphCompilationOptions

The option to debug layers during graph compilation.

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


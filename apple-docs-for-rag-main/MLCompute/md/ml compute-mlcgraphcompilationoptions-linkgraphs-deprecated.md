

- ML Compute
- MLCGraphCompilationOptions
-  linkGraphs Deprecated

Type Property

# linkGraphs

The option to link graphs during graph compilation.

iOS 14.0–17.4DeprecatediPadOS 14.0–17.4DeprecatedMac Catalyst 14.0–17.4DeprecatedmacOS 11.0–14.3DeprecatedtvOS 14.0–17.4Deprecated

``` source
static var linkGraphs: MLCGraphCompilationOptions { get }
```

## Discussion

Include this option when you link together one or more sub-graphs when executing the forward, gradient, and optimizer update. For example, if the full computation graph includes a layer that the framework doesn’t support, you’ll need to create multiple sub-graphs and link them together using `linkWithGraphs`. When doing so, include this option when you call `compileWithOptions` for graphs you want to link together.

## See Also

### Creating Graph Compilation Options

init(rawValue: UInt64)

Creates a graph compilation option with the specified raw value.

Deprecated

static var debugLayers: MLCGraphCompilationOptions

The option to debug layers during graph compilation.

Deprecated

static var disableLayerFusion: MLCGraphCompilationOptions

The option to disable layer fusion during graph compilation.

Deprecated

static var computeAllGradients: MLCGraphCompilationOptions

The option to compute all gradients during graph compilation.

Deprecated


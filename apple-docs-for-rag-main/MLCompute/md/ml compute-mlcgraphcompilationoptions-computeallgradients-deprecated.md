

- ML Compute
- MLCGraphCompilationOptions
-  computeAllGradients Deprecated

Type Property

# computeAllGradients

The option to compute all gradients during graph compilation.

iOS 14.0–17.4DeprecatediPadOS 14.0–17.4DeprecatedMac Catalyst 14.0–17.4DeprecatedmacOS 11.0–14.3DeprecatedtvOS 14.0–17.4Deprecated

``` source
static var computeAllGradients: MLCGraphCompilationOptions { get }
```

## Discussion

Include this option to compute gradients for layers with or without parameters that only take input tensors.

For example, if the first layer of a graph is a convolution layer, the framework only computes the gradients for weights and biases associated with the convolution layer, but not the gradients for the input. Include this option if you want to compute all gradients for the input.

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

static var linkGraphs: MLCGraphCompilationOptions

The option to link graphs during graph compilation.

Deprecated


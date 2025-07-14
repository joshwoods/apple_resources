

- ML Compute
-  MLCGraphCompilationOptions Deprecated

Structure

# MLCGraphCompilationOptions

A bitmask that specifies the options you use when compiling a graph.

iOS 14.0–17.4DeprecatediPadOS 14.0–17.4DeprecatedMac Catalyst 14.0–17.4DeprecatedmacOS 11.0–14.3DeprecatedtvOS 14.0–17.4Deprecated

``` source
struct MLCGraphCompilationOptions
```

## Topics

### Creating Graph Compilation Options

init(rawValue: UInt64)

Creates a graph compilation option with the specified raw value.

static var debugLayers: MLCGraphCompilationOptions

The option to debug layers during graph compilation.

static var disableLayerFusion: MLCGraphCompilationOptions

The option to disable layer fusion during graph compilation.

static var linkGraphs: MLCGraphCompilationOptions

The option to link graphs during graph compilation.

static var computeAllGradients: MLCGraphCompilationOptions

The option to compute all gradients during graph compilation.

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- ExpressibleByArrayLiteral
- OptionSet
- RawRepresentable
- Sendable
- SetAlgebra

## See Also

### Preparing Inference Graphs

func addInputs([String : MLCTensor]) -> Bool

Adds the inputs you specify to the inference graph.

Deprecated

func addInputs([String : MLCTensor], lossLabels: [String : MLCTensor]?, lossLabelWeights: [String : MLCTensor]?) -> Bool

Adds the inputs, loss labels, and loss label weights that you specify to the inference graph.

Deprecated

func addOutputs([String : MLCTensor]) -> Bool

Adds the outputs you specify to the inference graph.

Deprecated

func compile(options: MLCGraphCompilationOptions, device: MLCDevice) -> Bool

Compiles the inference graph for the options and device you specify.

Deprecated

func compile(options: MLCGraphCompilationOptions, device: MLCDevice, inputTensors: [String : MLCTensor]?, inputTensorsData: [String : MLCTensorData]?) -> Bool

Compiles the inference graph for the options, device, and input tensors you specify.

Deprecated

func link(with: [MLCInferenceGraph]) -> Bool

Links the inference graphs you specify.

Deprecated


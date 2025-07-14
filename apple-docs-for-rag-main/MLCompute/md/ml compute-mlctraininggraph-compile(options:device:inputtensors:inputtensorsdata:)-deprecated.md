

- ML Compute
- MLCTrainingGraph
-  compile(options:device:inputTensors:inputTensorsData:) Deprecated

Instance Method

# compile(options:device:inputTensors:inputTensorsData:)

Compiles the training graph for the options, device, and input tensors you specify.

iOS 14.5–17.4DeprecatediPadOS 14.5–17.4DeprecatedMac Catalyst 14.5–17.4DeprecatedmacOS 11.3–14.3DeprecatedtvOS 14.5–17.4Deprecated

``` source
func compile(
    options: MLCGraphCompilationOptions = [],
    device: MLCDevice,
    inputTensors: [String : MLCTensor]?,
    inputTensorsData: [String : MLCTensorData]?
) -> Bool
```

## Parameters 

`options`  

The compiler options.

`device`  

The device.

`inputTensors`  

The list of input tensors that are constants.

`inputTensorsData`  

The tensor data to use with the input tensors.

## Return Value

A Boolean that indicates success or failure.

## Discussion

If you specify the list of constant tensors before the framework compiles the graph, then the framework can perform additional optimizations during the compilation.

## See Also

### Preparing Training Graphs

func addInputs([String : MLCTensor], lossLabels: [String : MLCTensor]?) -> Bool

Adds the inputs and loss label inputs that you specify to the training graph.

Deprecated

func addInputs([String : MLCTensor], lossLabels: [String : MLCTensor]?, lossLabelWeights: [String : MLCTensor]?) -> Bool

Adds the inputs, loss labels, and loss label weights that you specify to the training graph.

Deprecated

func addOutputs([String : MLCTensor]) -> Bool

Adds the outputs to the training graph you specify.

Deprecated

func stopGradient(for: [MLCTensor]) -> Bool

Adds the tensors that you specify, to indicate which contributions the graph excludes when computing gradients during gradient pass.

Deprecated

func compileOptimizer(MLCOptimizer) -> Bool

Compiles the optimizer to use with a training graph you specify.

Deprecated

func compile(options: MLCGraphCompilationOptions, device: MLCDevice) -> Bool

Compiles the training graph for the options and device you specify.

Deprecated

func link(with: [MLCTrainingGraph]) -> Bool

Links the training graphs you specify.

Deprecated

func allocateUserGradient(for: MLCTensor) -> MLCTensor?

Allocates an entry for a gradient for the result tensor you specify.

Deprecated

struct MLCGraphCompilationOptions

A bitmask that specifies the options you use when compiling a graph.

Deprecated




- ML Compute
- MLCTrainingGraph
-  addInputs(\_:lossLabels:lossLabelWeights:) Deprecated

Instance Method

# addInputs(\_:lossLabels:lossLabelWeights:)

Adds the inputs, loss labels, and loss label weights that you specify to the training graph.

iOS 14.0–17.4DeprecatediPadOS 14.0–17.4DeprecatedMac Catalyst 14.0–17.4DeprecatedmacOS 11.0–14.3DeprecatedtvOS 14.0–17.4Deprecated

``` source
func addInputs(
    _ inputs: [String : MLCTensor],
    lossLabels: [String : MLCTensor]?,
    lossLabelWeights: [String : MLCTensor]?
) -> Bool
```

## Parameters 

`inputs`  

A dictionary that contains inputs.

`lossLabels`  

A dictionary that contains loss label inputs.

`lossLabelWeights`  

A dictionary that contains loss label weights.

## Return Value

`true` if the operation was successful.

## Discussion

Each input, loss label, or label weights tensor has a string identifier. When you execute the training graph, the string identifies which data object is the input for each tensor whose device memory requires updating before the framework actually executes the graph.

## See Also

### Preparing Training Graphs

func addInputs([String : MLCTensor], lossLabels: [String : MLCTensor]?) -> Bool

Adds the inputs and loss label inputs that you specify to the training graph.

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

func compile(options: MLCGraphCompilationOptions, device: MLCDevice, inputTensors: [String : MLCTensor]?, inputTensorsData: [String : MLCTensorData]?) -> Bool

Compiles the training graph for the options, device, and input tensors you specify.

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




- ML Compute
- MLCTrainingGraph
-  link(with:) Deprecated

Instance Method

# link(with:)

Links the training graphs you specify.

iOS 14.0–17.4DeprecatediPadOS 14.0–17.4DeprecatedMac Catalyst 14.0–17.4DeprecatedmacOS 11.0–14.3DeprecatedtvOS 14.0–17.4Deprecated

``` source
func link(with graphs: [MLCTrainingGraph]) -> Bool
```

## Parameters 

`graphs`  

An array that contains the training graphs.

## Return Value

`true` if the operation was successful.

## Discussion

When there are tensors shared by one or more layers in multiple sub-graphs, use this method to link subsequent training graphs with the first training sub-graph.

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

func compile(options: MLCGraphCompilationOptions, device: MLCDevice, inputTensors: [String : MLCTensor]?, inputTensorsData: [String : MLCTensorData]?) -> Bool

Compiles the training graph for the options, device, and input tensors you specify.

Deprecated

func allocateUserGradient(for: MLCTensor) -> MLCTensor?

Allocates an entry for a gradient for the result tensor you specify.

Deprecated

struct MLCGraphCompilationOptions

A bitmask that specifies the options you use when compiling a graph.

Deprecated


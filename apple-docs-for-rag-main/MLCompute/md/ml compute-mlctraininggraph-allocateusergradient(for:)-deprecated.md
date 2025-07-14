

- ML Compute
- MLCTrainingGraph
-  allocateUserGradient(for:) Deprecated

Instance Method

# allocateUserGradient(for:)

Allocates an entry for a gradient for the result tensor you specify.

iOS 14.0–17.4DeprecatediPadOS 14.0–17.4DeprecatedMac Catalyst 14.0–17.4DeprecatedmacOS 11.0–14.3DeprecatedtvOS 14.0–17.4Deprecated

``` source
func allocateUserGradient(for tensor: MLCTensor) -> MLCTensor?
```

## Parameters 

`tensor`  

A result tensor.

## Return Value

A gradient tensor.

## Discussion

Third-party numeric libraries can perform additional computations on the result tensor produced by a layer in the training graph. This external computation may produce gradients that you can backpropagate during gradient execution by using this method to allocate an entry for the gradient.

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

func link(with: [MLCTrainingGraph]) -> Bool

Links the training graphs you specify.

Deprecated

struct MLCGraphCompilationOptions

A bitmask that specifies the options you use when compiling a graph.

Deprecated


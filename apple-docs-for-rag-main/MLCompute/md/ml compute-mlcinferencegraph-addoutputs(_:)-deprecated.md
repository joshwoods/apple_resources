

- ML Compute
- MLCInferenceGraph
-  addOutputs(\_:) Deprecated

Instance Method

# addOutputs(\_:)

Adds the outputs you specify to the inference graph.

iOS 14.0–17.4DeprecatediPadOS 14.0–17.4DeprecatedMac Catalyst 14.0–17.4DeprecatedmacOS 11.0–14.3DeprecatedtvOS 14.0–17.4Deprecated

``` source
func addOutputs(_ outputs: [String : MLCTensor]) -> Bool
```

## Parameters 

`outputs`  

A dictionary containing outputs.

## Return Value

I`true` if the operation was successful.

## See Also

### Preparing Inference Graphs

func addInputs([String : MLCTensor]) -> Bool

Adds the inputs you specify to the inference graph.

Deprecated

func addInputs([String : MLCTensor], lossLabels: [String : MLCTensor]?, lossLabelWeights: [String : MLCTensor]?) -> Bool

Adds the inputs, loss labels, and loss label weights that you specify to the inference graph.

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

struct MLCGraphCompilationOptions

A bitmask that specifies the options you use when compiling a graph.

Deprecated


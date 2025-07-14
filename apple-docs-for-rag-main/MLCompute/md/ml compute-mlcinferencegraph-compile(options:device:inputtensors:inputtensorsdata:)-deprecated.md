

- ML Compute
- MLCInferenceGraph
-  compile(options:device:inputTensors:inputTensorsData:) Deprecated

Instance Method

# compile(options:device:inputTensors:inputTensorsData:)

Compiles the inference graph for the options, device, and input tensors you specify.

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

func link(with: [MLCInferenceGraph]) -> Bool

Links the inference graphs you specify.

Deprecated

struct MLCGraphCompilationOptions

A bitmask that specifies the options you use when compiling a graph.

Deprecated


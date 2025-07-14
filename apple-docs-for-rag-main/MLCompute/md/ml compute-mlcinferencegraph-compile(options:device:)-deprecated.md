

- ML Compute
- MLCInferenceGraph
-  compile(options:device:) Deprecated

Instance Method

# compile(options:device:)

Compiles the inference graph for the options and device you specify.

iOS 14.0–17.4DeprecatediPadOS 14.0–17.4DeprecatedMac Catalyst 14.0–17.4DeprecatedmacOS 11.0–14.3DeprecatedtvOS 14.0–17.4Deprecated

``` source
func compile(
    options: MLCGraphCompilationOptions = [],
    device: MLCDevice
) -> Bool
```

## Parameters 

`options`  

The compiler options.

`device`  

The device.

## Return Value

`true` if the operation was successful.

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

func compile(options: MLCGraphCompilationOptions, device: MLCDevice, inputTensors: [String : MLCTensor]?, inputTensorsData: [String : MLCTensorData]?) -> Bool

Compiles the inference graph for the options, device, and input tensors you specify.

Deprecated

func link(with: [MLCInferenceGraph]) -> Bool

Links the inference graphs you specify.

Deprecated

struct MLCGraphCompilationOptions

A bitmask that specifies the options you use when compiling a graph.

Deprecated


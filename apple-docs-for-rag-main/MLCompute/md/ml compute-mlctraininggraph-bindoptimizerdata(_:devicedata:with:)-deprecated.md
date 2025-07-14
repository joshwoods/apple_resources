

- ML Compute
- MLCTrainingGraph
-  bindOptimizerData(\_:deviceData:with:) Deprecated

Instance Method

# bindOptimizerData(\_:deviceData:with:)

Associates the optimizer and device data you specify along with the tensor.

iOS 14.0–17.4DeprecatediPadOS 14.0–17.4DeprecatedMac Catalyst 14.0–17.4DeprecatedmacOS 11.0–14.3DeprecatedtvOS 14.0–17.4Deprecated

``` source
func bindOptimizerData(
    _ data: [MLCTensorData],
    deviceData: [MLCTensorOptimizerDeviceData]?,
    with tensor: MLCTensor
) -> Bool
```

## Parameters 

`data`  

The optimizer data that you want to associate with the tensor.

`deviceData`  

The optimizer device data that you want to associate with the tensor.

`tensor`  

The tensor that you want to associate the data with.

## Return Value

A Boolean value that indicates whether the data successfully associates with the tensor.

## See Also

### Inspecting Training Graphs

var optimizer: MLCOptimizer?

The optimizer to use with the training graph.

Deprecated

var deviceMemorySize: Int

The device memory size in bytes for all intermediate tensors for forward, gradient passes, and optimizer updates for all layers in the training graph.

Deprecated

func gradientTensor(forInput: MLCTensor) -> MLCTensor?

Gets the gradient tensor for the input tensor you specify.

Deprecated

func sourceGradientTensors(for: MLCLayer) -> [MLCTensor]

Gets the source gradient tensors for the layer in the training graph you specify.

Deprecated

func resultGradientTensors(for: MLCLayer) -> [MLCTensor]

Gets the result gradient tensors for the layer in the training graph you specify.

Deprecated

func gradientData(forParameter: MLCTensor, layer: MLCLayer) -> Data?

Gets the gradient data for the trainable parameter and associated layer you specify.

Deprecated


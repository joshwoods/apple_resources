

- ML Compute
- MLCTrainingGraph
-  gradientData(forParameter:layer:) Deprecated

Instance Method

# gradientData(forParameter:layer:)

Gets the gradient data for the trainable parameter and associated layer you specify.

iOS 14.0–17.4DeprecatediPadOS 14.0–17.4DeprecatedMac Catalyst 14.0–17.4DeprecatedmacOS 11.0–14.3DeprecatedtvOS 14.0–17.4Deprecated

``` source
func gradientData(
    forParameter parameter: MLCTensor,
    layer: MLCLayer
) -> Data?
```

## Parameters 

`parameter`  

The trainable parameter you associated with the layer.

`layer`  

A layer in the training graph.

## Return Value

The gradient data, or `nil`.

## Discussion

The layer must be an instance one of the following types:

- MLCConvolutionLayer

- MLCFullyConnectedLayer

- MLCBatchNormalizationLayer

- MLCInstanceNormalizationLayer

- MLCGroupNormalizationLayer

- MLCLayerNormalizationLayer

Note

This method returns `nil` if the layer isn’t trainable or you didn’t execute the training graph with separate calls to forward and gradient passes.

## See Also

### Inspecting Training Graphs

func bindOptimizerData([MLCTensorData], deviceData: [MLCTensorOptimizerDeviceData]?, with: MLCTensor) -> Bool

Associates the optimizer and device data you specify along with the tensor.

Deprecated

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


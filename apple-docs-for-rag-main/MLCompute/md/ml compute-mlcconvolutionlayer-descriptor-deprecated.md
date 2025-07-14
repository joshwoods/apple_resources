

- ML Compute
- MLCConvolutionLayer
-  descriptor Deprecated

Instance Property

# descriptor

The configuration object you use to create the convolution layer.

iOS 14.0–17.4DeprecatediPadOS 14.0–17.4DeprecatedMac Catalyst 14.0–17.4DeprecatedmacOS 11.0–14.3DeprecatedtvOS 14.0–17.4Deprecated

``` source
@NSCopying
var descriptor: MLCConvolutionDescriptor { get }
```

## See Also

### Inspecting Convolution Layers

var weights: MLCTensor

The weights tensor you use for the convolution layer.

Deprecated

var biases: MLCTensor?

The biases tensor you use for the convolution layer.

Deprecated

var weightsParameter: MLCTensorParameter

The weights tensor parameter you use for optimizer updates.

Deprecated

var biasesParameter: MLCTensorParameter?

The biases tensor parameter you use for optimizer updates.

Deprecated


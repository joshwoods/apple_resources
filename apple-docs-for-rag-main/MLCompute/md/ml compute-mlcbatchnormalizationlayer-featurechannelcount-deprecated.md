

- ML Compute
- MLCBatchNormalizationLayer
-  featureChannelCount Deprecated

Instance Property

# featureChannelCount

The number of feature channels.

iOS 14.0–17.4DeprecatediPadOS 14.0–17.4DeprecatedMac Catalyst 14.0–17.4DeprecatedmacOS 11.0–14.3DeprecatedtvOS 14.0–17.4Deprecated

``` source
var featureChannelCount: Int { get }
```

## See Also

### Inspecting Batch Normalization Layers

var mean: MLCTensor

The mean tensor.

Deprecated

var variance: MLCTensor

The variance tensor.

Deprecated

var beta: MLCTensor?

The beta tensor.

Deprecated

var gamma: MLCTensor?

The gamma tensor.

Deprecated

var varianceEpsilon: Float

The variance epsilon you use for numerical stability.

Deprecated

var momentum: Float

The value you use for the running mean and variance computation.

Deprecated

var betaParameter: MLCTensorParameter?

The beta tensor parameter you use for optimizer updates.

Deprecated

var gammaParameter: MLCTensorParameter?

The gamma tensor parameter you use for optimizer updates.

Deprecated


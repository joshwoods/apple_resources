

- ML Compute
- MLCInstanceNormalizationLayer
-  gamma Deprecated

Instance Property

# gamma

The gamma tensor.

iOS 14.0–17.4DeprecatediPadOS 14.0–17.4DeprecatedMac Catalyst 14.0–17.4DeprecatedmacOS 11.0–14.3DeprecatedtvOS 14.0–17.4Deprecated

``` source
var gamma: MLCTensor? { get }
```

## See Also

### Inspecting Instance Normalization Layers

var beta: MLCTensor?

The beta tensor.

Deprecated

var betaParameter: MLCTensorParameter?

The beta tensor parameter you use for optimizer updates.

Deprecated

var featureChannelCount: Int

The number of feature channels.

Deprecated

var gammaParameter: MLCTensorParameter?

The gamma tensor parameter you use for optimizer updates.

Deprecated

var mean: MLCTensor?

The running mean tensor.

Deprecated

var momentum: Float

The momentum value for the running mean and variance computation.

Deprecated

var variance: MLCTensor?

The running variance tensor.

Deprecated

var varianceEpsilon: Float

The variance epsilon you use for numerical stability.

Deprecated


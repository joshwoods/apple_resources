

- ML Compute
- MLCLayerNormalizationLayer
-  betaParameter Deprecated

Instance Property

# betaParameter

The beta tensor parameter you use for optimizer updates.

iOS 14.0–17.4DeprecatediPadOS 14.0–17.4DeprecatedMac Catalyst 14.0–17.4DeprecatedmacOS 11.0–14.3DeprecatedtvOS 14.0–17.4Deprecated

``` source
var betaParameter: MLCTensorParameter? { get }
```

## See Also

### Inspecting Layer Normalization Layers

var normalizedShape: [Int]

The shape of the axes where normalization occurs.

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

var gammaParameter: MLCTensorParameter?

The gamma tensor parameter you use for optimizer updates.

Deprecated




- ML Compute
- MLCLayerNormalizationLayer
-  varianceEpsilon Deprecated

Instance Property

# varianceEpsilon

The variance epsilon you use for numerical stability.

iOS 14.0–17.4DeprecatediPadOS 14.0–17.4DeprecatedMac Catalyst 14.0–17.4DeprecatedmacOS 11.0–14.3DeprecatedtvOS 14.0–17.4Deprecated

``` source
var varianceEpsilon: Float { get }
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

var betaParameter: MLCTensorParameter?

The beta tensor parameter you use for optimizer updates.

Deprecated

var gammaParameter: MLCTensorParameter?

The gamma tensor parameter you use for optimizer updates.

Deprecated


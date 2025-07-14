

- ML Compute
- MLCLayerNormalizationLayer
-  normalizedShape Deprecated

Instance Property

# normalizedShape

The shape of the axes where normalization occurs.

iOS 14.0–17.0DeprecatediPadOS 14.0–17.0DeprecatedMac Catalyst 14.0–17.0DeprecatedmacOS 11.0–14.0DeprecatedtvOS 14.0–17.0Deprecated

``` source
var normalizedShape: [Int] { get }
```

Deprecated

Use Metal Performance Shaders Graph or BNNS instead.

## Discussion

Define the shape of the axes in the dimensions `[w]`, `[h, w]`, or `[c, h, w]`, where `w` is width, `h` is height, and `c` is channel count.

## See Also

### Inspecting Layer Normalization Layers

var beta: MLCTensor?

The beta tensor.

Deprecated

var gamma: MLCTensor?

The gamma tensor.

Deprecated

var varianceEpsilon: Float

The variance epsilon you use for numerical stability.

Deprecated

var betaParameter: MLCTensorParameter?

The beta tensor parameter you use for optimizer updates.

Deprecated

var gammaParameter: MLCTensorParameter?

The gamma tensor parameter you use for optimizer updates.

Deprecated


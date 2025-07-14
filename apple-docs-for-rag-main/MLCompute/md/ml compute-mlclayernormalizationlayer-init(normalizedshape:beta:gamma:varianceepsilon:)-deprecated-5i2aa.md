

- ML Compute
- MLCLayerNormalizationLayer
-  init(normalizedShape:beta:gamma:varianceEpsilon:) Deprecated

Initializer

# init(normalizedShape:beta:gamma:varianceEpsilon:)

Creates a normalization layer with a shape, beta and gamma tensors, and variance epsilon you specify.

iOS 14.0–17.0DeprecatediPadOS 14.0–17.0DeprecatedMac Catalyst 14.0–17.0DeprecatedmacOS 11.0–14.0DeprecatedtvOS 14.0–17.0Deprecated

``` source
convenience init?(
    normalizedShape: [Int],
    beta: MLCTensor,
    gamma: MLCTensor,
    varianceEpsilon: Float
)
```

Deprecated

Use Metal Performance Shaders Graph or BNNS instead.

## Parameters 

`normalizedShape`  

The shape of the axes where normalization occurs.

`beta`  

The beta tensor.

`gamma`  

The gamma tensor.

`varianceEpsilon`  

The variance epsilon you use for numerical stability.

## See Also

### Creating Layer Normalization Layers

convenience init?(normalizedShape: [Int], beta: MLCTensor?, gamma: MLCTensor?, varianceEpsilon: Float)

Creates a normalization layer with a shape, optional beta and gamma tensors, and variance epsilon you specify.

Deprecated


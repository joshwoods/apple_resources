

- ML Compute
- MLCInstanceNormalizationLayer
-  init(featureChannelCount:beta:gamma:varianceEpsilon:) Deprecated

Initializer

# init(featureChannelCount:beta:gamma:varianceEpsilon:)

Creates an instance normalization layer with the number of feature channels, beta and gamma tensors, and variance epsilon you specify.

iOS 14.0–17.4DeprecatediPadOS 14.0–17.4DeprecatedMac Catalyst 14.0–17.4DeprecatedmacOS 11.0–14.3DeprecatedtvOS 14.0–17.4Deprecated

``` source
convenience init?(
    featureChannelCount: Int,
    beta: MLCTensor?,
    gamma: MLCTensor?,
    varianceEpsilon: Float
)
```

## Parameters 

`featureChannelCount`  

The number of feature channels.

`beta`  

The beta tensor.

`gamma`  

The gamma tensor.

`varianceEpsilon`  

The variance epsilon you use for numerical stability.

## See Also

### Creating Instance Normalization Layers

convenience init?(featureChannelCount: Int, beta: MLCTensor?, gamma: MLCTensor?, varianceEpsilon: Float, momentum: Float)

Creates an instance normalization layer with the number of feature channels, beta and gamma tensors, variance epsilon, and momentum you specify.

Deprecated

convenience init?(featureChannelCount: Int, mean: MLCTensor, variance: MLCTensor, beta: MLCTensor?, gamma: MLCTensor?, varianceEpsilon: Float, momentum: Float)

Creates an instance normalization layer with the number of feature channels, mean, variance, beta and gamma tensors, variance epsilon, and momentum you specify.

Deprecated


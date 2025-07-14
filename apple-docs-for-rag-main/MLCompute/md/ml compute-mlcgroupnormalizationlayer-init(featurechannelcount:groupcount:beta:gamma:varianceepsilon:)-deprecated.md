

- ML Compute
- MLCGroupNormalizationLayer
-  init(featureChannelCount:groupCount:beta:gamma:varianceEpsilon:) Deprecated

Initializer

# init(featureChannelCount:groupCount:beta:gamma:varianceEpsilon:)

Creates a group normalization layer with the number of feature channels and groups, beta and gamma tensors, and variance epsilon you specify.

iOS 14.0–17.4DeprecatediPadOS 14.0–17.4DeprecatedMac Catalyst 14.0–17.4DeprecatedmacOS 11.0–14.3DeprecatedtvOS 14.0–17.4Deprecated

``` source
convenience init?(
    featureChannelCount: Int,
    groupCount: Int,
    beta: MLCTensor?,
    gamma: MLCTensor?,
    varianceEpsilon: Float
)
```

## Parameters 

`featureChannelCount`  

The number of feature channels.

`groupCount`  

The number of groups into which you separate the channels.

`beta`  

The beta tensor.

`gamma`  

The gamma tensor.

`varianceEpsilon`  

The variance epsilon you use for numerical stability.


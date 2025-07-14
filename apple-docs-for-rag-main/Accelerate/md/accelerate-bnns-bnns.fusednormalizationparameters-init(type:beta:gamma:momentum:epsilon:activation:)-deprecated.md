

- Accelerate
- BNNS
- BNNS.FusedNormalizationParameters
-  init(type:beta:gamma:momentum:epsilon:activation:) Deprecated

Initializer

# init(type:beta:gamma:momentum:epsilon:activation:)

Returns a new fused normalization parameters structure.

iOS 15.0+iPadOS 15.0+Mac CatalystmacOS 12.0+visionOSwatchOS 8.0+tvOS 15.0+

``` source
init(
    type: BNNS.NormalizationType,
    beta: BNNSNDArrayDescriptor? = nil,
    gamma: BNNSNDArrayDescriptor? = nil,
    momentum: Float = 0,
    epsilon: Float,
    activation: BNNS.ActivationFunction
)
```

Deprecated

Use the BNNSGraph API instead.

## Parameters 

`type`  

An enumeration that specifies the normalization type.

`beta`  

The descriptor of the beta.

`gamma`  

The descriptor of the gamma.

`momentum`  

A value, between 0 and 1, the normalization operation uses to update the moving mean and moving variance during training.

`epsilon`  

The epsilon in the computation of the standard deviation.

`activation`  

The activation function that the layer applies to the output.




- ML Compute
- MLCLossDescriptor
-  init(type:reductionType:weight:) Deprecated

Initializer

# init(type:reductionType:weight:)

Creates a loss descriptor with the loss function, reduction type, and weight you specify.

iOS 14.0–17.4DeprecatediPadOS 14.0–17.4DeprecatedMac Catalyst 14.0–17.4DeprecatedmacOS 11.0–14.3DeprecatedtvOS 14.0–17.4Deprecated

``` source
convenience init(
    type lossType: MLCLossType,
    reductionType: MLCReductionType,
    weight: Float
)
```

## Parameters 

`lossType`  

The loss function type.

`reductionType`  

The reduction operation type.

`weight`  

A scalar floating-point weight value.

## See Also

### Creating Loss Descriptors

convenience init(type: MLCLossType, reductionType: MLCReductionType)

Creates a loss descriptor with the loss function and reduction type you specify.

Deprecated

convenience init(type: MLCLossType, reductionType: MLCReductionType, weight: Float, labelSmoothing: Float, classCount: Int)

Creates a loss descriptor with the loss function, reduction type, weight, label smoothing, and number of classes you specify.

Deprecated

convenience init(type: MLCLossType, reductionType: MLCReductionType, weight: Float, labelSmoothing: Float, classCount: Int, epsilon: Float, delta: Float)

Creates a loss descriptor with the loss function, reduction type, weight, label smoothing, and number of classes, epsilon, and delta that you specify.

Deprecated


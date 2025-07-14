

- ML Compute
- MLCReductionLayer
-  init(reductionType:dimensions:) Deprecated

Initializer

# init(reductionType:dimensions:)

Creates a reduction layer using the reduction type and dimensions you specify.

iOS 14.5–17.0DeprecatediPadOS 14.5–17.0DeprecatedMac Catalyst 14.5–17.0DeprecatedmacOS 11.3–14.0DeprecatedtvOS 14.5–17.0Deprecated

``` source
convenience init?(
    reductionType: MLCReductionType,
    dimensions: [Int]
)
```

Deprecated

Use Metal Performance Shaders Graph or BNNS instead.

## Parameters 

`reductionType`  

The reduction type.

`dimensions`  

The dimensions to perform the reduction operation on.

## See Also

### Creating Reduction Layers

convenience init?(reductionType: MLCReductionType, dimension: Int)

Creates a reduction layer using the reduction type and dimension you specify.

Deprecated

enum MLCReductionType

Constants that describe a reduction operation type.

Deprecated




- ML Compute
- MLCReductionLayer
-  init(reductionType:dimension:) Deprecated

Initializer

# init(reductionType:dimension:)

Creates a reduction layer using the reduction type and dimension you specify.

iOS 14.0–17.4DeprecatediPadOS 14.0–17.4DeprecatedMac Catalyst 14.0–17.4DeprecatedmacOS 11.0–14.3DeprecatedtvOS 14.0–17.4Deprecated

``` source
convenience init?(
    reductionType: MLCReductionType,
    dimension: Int
)
```

## Parameters 

`reductionType`  

The reduction type.

`dimension`  

The dimension to perform the reduction operation on.

## Return Value

A new MLCReductionLayer instance.

## See Also

### Creating Reduction Layers

convenience init?(reductionType: MLCReductionType, dimensions: [Int])

Creates a reduction layer using the reduction type and dimensions you specify.

Deprecated

enum MLCReductionType

Constants that describe a reduction operation type.

Deprecated


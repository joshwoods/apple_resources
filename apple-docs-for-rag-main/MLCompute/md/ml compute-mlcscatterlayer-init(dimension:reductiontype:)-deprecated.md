

- ML Compute
- MLCScatterLayer
-  init(dimension:reductionType:) Deprecated

Initializer

# init(dimension:reductionType:)

Creates a scatter layer with the dimension and reduction type you specify.

iOS 14.5–17.4DeprecatediPadOS 14.5–17.4DeprecatedMac Catalyst 14.5–17.4DeprecatedmacOS 11.3–14.3DeprecatedtvOS 14.5–17.4Deprecated

``` source
convenience init?(
    dimension: Int,
    reductionType: MLCReductionType
)
```

## Parameters 

`dimension`  

The dimension to index.

`reductionType`  

The reduction type that applies to all values in a source tensor.

## Discussion

Important

The reduction type can be either MLCReductionType.none or MLCReductionType.sum.


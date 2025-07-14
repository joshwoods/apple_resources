

- ML Compute
- MLCSplitLayer
-  init(splitCount:dimension:) Deprecated

Initializer

# init(splitCount:dimension:)

Creates a split layer with the number of splits and dimension you specify.

iOS 14.0–17.4DeprecatediPadOS 14.0–17.4DeprecatedMac Catalyst 14.0–17.4DeprecatedmacOS 11.0–14.3DeprecatedtvOS 14.0–17.4Deprecated

``` source
convenience init(
    splitCount: Int,
    dimension: Int
)
```

## Parameters 

`splitCount`  

The number of splits.

`dimension`  

The dimension or axis along which to split the tensor.

## See Also

### Creating Split Layers

convenience init(splitSectionLengths: [Int], dimension: Int)

Creates a split layer with the lengths of each split section and dimension you specify.

Deprecated


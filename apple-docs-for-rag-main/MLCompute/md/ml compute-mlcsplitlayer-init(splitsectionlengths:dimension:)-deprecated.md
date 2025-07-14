

- ML Compute
- MLCSplitLayer
-  init(splitSectionLengths:dimension:) Deprecated

Initializer

# init(splitSectionLengths:dimension:)

Creates a split layer with the lengths of each split section and dimension you specify.

iOS 14.0–17.0DeprecatediPadOS 14.0–17.0DeprecatedMac Catalyst 14.0–17.0DeprecatedmacOS 11.0–14.0DeprecatedtvOS 14.0–17.0Deprecated

``` source
convenience init(
    splitSectionLengths: [Int],
    dimension: Int
)
```

Deprecated

Use Metal Performance Shaders Graph or BNNS instead.

## Parameters 

`splitSectionLengths`  

An array that contains the lengths of each split section.

`dimension`  

The dimension or axis along which to split the tensor.

## See Also

### Creating Split Layers

convenience init(splitCount: Int, dimension: Int)

Creates a split layer with the number of splits and dimension you specify.

Deprecated


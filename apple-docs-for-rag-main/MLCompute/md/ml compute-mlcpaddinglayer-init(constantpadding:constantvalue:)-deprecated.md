

- ML Compute
- MLCPaddingLayer
-  init(constantPadding:constantValue:) Deprecated

Initializer

# init(constantPadding:constantValue:)

Creates a padding layer with the constant padding sizes and constant value you specify.

iOS 14.0–17.0DeprecatediPadOS 14.0–17.0DeprecatedMac Catalyst 14.0–17.0DeprecatedmacOS 11.0–14.0DeprecatedtvOS 14.0–17.0Deprecated

``` source
convenience init(
    constantPadding: [Int],
    constantValue: Float
)
```

Deprecated

Use Metal Performance Shaders Graph or BNNS instead.

## Parameters 

`constantPadding`  

An array that contains the constant padding sizes.

`constantValue`  

The constant value you use to pad the source tensor.

## See Also

### Creating Padding Layers

convenience init(reflectionPadding: [Int])

Creates a padding layer with the reflection padding sizes you specify.

Deprecated

convenience init(symmetricPadding: [Int])

Creates a padding layer with the symmetric padding sizes you specify.

Deprecated

convenience init(zeroPadding: [Int])

Creates a padding layer with the zero padding sizes you specify.

Deprecated


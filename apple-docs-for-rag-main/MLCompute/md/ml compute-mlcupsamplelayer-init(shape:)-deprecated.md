

- ML Compute
- MLCUpsampleLayer
-  init(shape:) Deprecated

Initializer

# init(shape:)

Creates an upsample layer with the shape you specify.

iOS 14.0–17.0DeprecatediPadOS 14.0–17.0DeprecatedMac Catalyst 14.0–17.0DeprecatedmacOS 11.0–14.0DeprecatedtvOS 14.0–17.0Deprecated

``` source
convenience init?(shape: [Int])
```

Deprecated

Use Metal Performance Shaders Graph or BNNS instead.

## Parameters 

`shape`  

An array that contains the dimensions of the result tensor.

## See Also

### Creating Upsample Layers

convenience init?(shape: [Int], sampleMode: MLCSampleMode, alignsCorners: Bool)

Creates an upsample layer with the shape, upsampling algorithm, and corner alignment option you specify.

Deprecated

enum MLCSampleMode

A sampling mode for an upsample layer.

Deprecated


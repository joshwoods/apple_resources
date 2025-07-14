

- ML Compute
- MLCUpsampleLayer
-  init(shape:sampleMode:alignsCorners:) Deprecated

Initializer

# init(shape:sampleMode:alignsCorners:)

Creates an upsample layer with the shape, upsampling algorithm, and corner alignment option you specify.

iOS 14.0–17.0DeprecatediPadOS 14.0–17.0DeprecatedMac Catalyst 14.0–17.0DeprecatedmacOS 11.0–14.0DeprecatedtvOS 14.0–17.0Deprecated

``` source
convenience init?(
    shape: [Int],
    sampleMode: MLCSampleMode,
    alignsCorners: Bool
)
```

Deprecated

Use Metal Performance Shaders Graph or BNNS instead.

## Parameters 

`shape`  

An array representing the dimensions of the result tensor.

`sampleMode`  

The upsampling algorithm type; the default value is nearest.

`alignsCorners`  

A Boolean that indicates whether the layer aligns the corner pixels of the input and output tensors.

## See Also

### Creating Upsample Layers

convenience init?(shape: [Int])

Creates an upsample layer with the shape you specify.

Deprecated

enum MLCSampleMode

A sampling mode for an upsample layer.

Deprecated


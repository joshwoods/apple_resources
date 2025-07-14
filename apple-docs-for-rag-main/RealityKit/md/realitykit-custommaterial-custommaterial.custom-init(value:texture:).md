

- RealityKit
- CustomMaterial
- CustomMaterial.Custom
-  init(value:texture:) 

Initializer

# init(value:texture:)

Creates a custom object from a vector and texture.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+

``` source
init(
    value: SIMD4 = .init(repeating: 0),
    texture: CustomMaterial.Texture? = nil
)
```

## Parameters 

`value`  

A four-component vector.

`texture`  

An optional texture.

## Discussion

Use this initializer to create a new CustomMaterial.Custom object from a four-component vector, a texture, or both. RealityKit passes these values automatically to your custom material’s shader functions. Custom values have no predefined meaning, and RealityKit doesn’t use them other than to make them available in your surface shader and geometry modifier.


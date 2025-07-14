

- RealityKit
- CustomMaterial
- CustomMaterial.BaseColor
-  init(\_:) 

Initializer

# init(\_:)

Creates a custom base color object from an existing physically based material’s base color object.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+

``` source
init(_ value: PhysicallyBasedMaterial.BaseColor)
```

## Parameters 

`value`  

The base color object from a physically based material.

## Discussion

Use this initializer to create a CustomMaterial.BaseColor that contains the same tint and texture values as an existing PhysicallyBasedMaterial.BaseColor object.

Both `tint` and `texture` from the PhysicallyBasedMaterial.BaseColor object are available in your surface shader, but RealityKit doesn’t automatically use those values to render the entity. Your surface shader needs to calculate the final base color value for each pixel and assign it by calling `params.surface().set_base_color()`.

For more information on creating custom materials and writing shader functions, see Modifying RealityKit rendering using custom materials.

## See Also

### Creating a base color object

init(tint: UIColor, texture: CustomMaterial.Texture?)

Creates a base color object from a color or texture on macOS.

init(tint: NSColor, texture: CustomMaterial.Texture?)

Creates a base color object from a color or texture on macOS.


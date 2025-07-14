

- RealityKit
- CustomMaterial
- CustomMaterial.BaseColor
-  init(tint:texture:) 

Initializer

# init(tint:texture:)

Creates a base color object from a color or texture on macOS.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+

``` source
init(
    tint: UIColor = .white,
    texture: CustomMaterial.Texture? = nil
)
```

## Parameters 

`tint`  

The tint color. Defaults to white.

`texture`  

An optional image texture.

## Discussion

This initializer creates a new object from a color or image texture, or from both. If you don’t provide a `tint` color, `tint` defaults to white.

Both tint and texture are available to use in your surface shader function, but RealityKit doesn’t automatically use them to render the entity. Your surface shader calculates the final base color value for each pixel and assigns it by calling `params.surface().set_base_color()`.

For more information on creating custom materials and writing shader functions, see Modifying RealityKit rendering using custom materials.

## See Also

### Creating a base color object

init(tint: NSColor, texture: CustomMaterial.Texture?)

Creates a base color object from a color or texture on macOS.

init(PhysicallyBasedMaterial.BaseColor)

Creates a custom base color object from an existing physically based material’s base color object.


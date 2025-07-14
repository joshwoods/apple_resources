

- RealityKit
- PhysicallyBasedMaterial
- PhysicallyBasedMaterial.BaseColor
-  init(tint:texture:) 

Initializer

# init(tint:texture:)

Creates a base color object from a color or texture on macOS.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+visionOS

``` source
init(
    tint: UIColor = .white,
    texture: MaterialParameters.Texture? = nil
)
```

## Parameters 

`tint`  

The tint color. Defaults to white.

`texture`  

An optional image texture.

## Discussion

This initializer creates a new instance from a color or image texture, or from both. If you don’t provide a `tint` color, `tint` defaults to white.

If you specify `texture`, RealityKit calculates the final base color for the entity by UV-mapping `texture` onto the entity and then multiplying the color at any given pixel by `tint`. If `tint` is white, RealityKit renders the textured untinted.

If you don’t specify a texture, RealityKit uses `tint` as the entity’s base color.

## See Also

### Creating a base color object

init(tint: NSColor, texture: MaterialParameters.Texture?)

Creates a base color object from a color or texture on macOS.

init(CustomMaterial.BaseColor)

Creates a base color object from a custom material’s base color property.


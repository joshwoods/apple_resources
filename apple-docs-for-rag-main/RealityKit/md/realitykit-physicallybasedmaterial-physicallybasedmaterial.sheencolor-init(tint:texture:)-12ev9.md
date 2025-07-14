

- RealityKit
- PhysicallyBasedMaterial
- PhysicallyBasedMaterial.SheenColor
-  init(tint:texture:) 

Initializer

# init(tint:texture:)

Creates a sheen color in macOS.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+

``` source
init(
    tint: NSColor = .white,
    texture: MaterialParameters.Texture? = nil
)
```

## Parameters 

`tint`  

The tint color.

`texture`  

The optional image texture.

## Discussion

This initializer creates an object from a color, an image texture, or from both. If you don’t provide a `tint` color, `tint` defaults to white.

If you specify `texture`, RealityKit calculates the final sheen color for the entity by UV-mapping `texture` onto the entity and then multiplying the color at any given pixel by `tint`. If `tint` is white, RealityKit uses the texture untinted.

If you don’t specify `texture`, then RealityKit uses `tint` as the entity’s sheen color.

## See Also

### Creating a sheen color

init(tint: UIColor, texture: MaterialParameters.Texture?)

Creates a sheen color in macOS.


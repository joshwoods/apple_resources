

- RealityKit
- PhysicallyBasedMaterial
- PhysicallyBasedMaterial.Roughness
-  init(scale:texture:) 

Initializer

# init(scale:texture:)

Creates a roughness object from a color or texture.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+visionOS

``` source
init(
    scale: Float = 1.0,
    texture: PhysicallyBasedMaterial.Texture? = nil
)
```

## Parameters 

`scale`  

The roughness value.

`texture`  

An optional image texture.

## Discussion

The `roughness` property represents how much the surface of the entity scatters light it reflects. A material with a high roughness has a matte appearance, while one with a low roughness has a shiny appearance.

Use this initializer to create a new object from a single roughness value, from an image texture, or from both.

If you specify `texture`, RealityKit calculates the `roughness` for the entity by UV-mapping `texture` onto the entity and multiplying the value of each mapped pixel by `scale`. If you don’t specify `texture`, then RealityKit uses `scale` as the entire entity’s roughness. If you provide a color image for `texture` rather than a grayscale image, RealityKit only uses the intensity of the image’s red channel.

## See Also

### Creating a roughness object

init(floatLiteral: Float)

Creates an object from a single value.

init(CustomMaterial.Roughness)

Creates a roughness object from a custom material’s roughness property.


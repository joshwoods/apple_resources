

- RealityKit
- PhysicallyBasedMaterial
- PhysicallyBasedMaterial.Specular
-  init(scale:texture:) 

Initializer

# init(scale:texture:)

Creates an object from a single value or a texture.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+visionOS

``` source
init(
    scale: Float = 1.0,
    texture: PhysicallyBasedMaterial.Texture? = nil
)
```

## Parameters 

`scale`  

A value from 0.0 to 1.0 to use as the specular value for the material.

`texture`  

An optional UV-mapped image texture.

## Discussion

RealityKit automatically draws *specular highlights* for physically based materials using the values of various properties, primarily roughness and metallic. Specular highlights are bright spots of reflected light that appear on shiny objects.

While many real-world objects can be accurately and realistically simulated with just the core PBR properties, you can create additional realistic effects by augmenting the specular highlights.

This initializer creates a PhysicallyBasedMaterial.Specular object from a single value, an image texture, or both.

If you specify `texture`, RealityKit calculates the `specular` for the entity by UV-mapping `texture` onto the entity and multiplying the value of each mapped pixel by `scale`. If you don’t specify `texture`, RealityKit uses `scale` as the entire entity’s specular. If you provide a color image for `texture` rather than a grayscale image, RealityKit only uses the intensity of the image’s red channel.

## See Also

### Creating a specular object

init(floatLiteral: Float)

Creates an object from single value.

init(CustomMaterial.Specular)

Creates an object from a custom material’s specular property.


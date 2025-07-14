

- RealityKit
- PhysicallyBasedMaterial
- PhysicallyBasedMaterial.Clearcoat
-  init(scale:texture:) 

Initializer

# init(scale:texture:)

Creates a clearcoat object using a single value or a texture.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+visionOS

``` source
init(
    scale: Float = 1.0,
    texture: PhysicallyBasedMaterial.Texture? = nil
)
```

## Parameters 

`scale`  

The clearcoat value for the entire material.

`texture`  

The clearcoat values as the texture of a UV-mapped image.

## Discussion

A clearcoat is a separate layer of transparent specular highlights used to simulate a clear transparent coating, like the paint on a car, or the surface of lacquered objects. Use this initializer to create an object to specify the amount of clearcoat for a material using a single value for the entire material, a UV-mapped image to specify different values for different parts of the entity, or both.

If you specify `texture`, RealityKit calculates the clearcoat intensity for the entity by UV-mapping `texture` onto the entity and multiplying the value of each mapped pixel by `scale`. If you don’t specify `texture`, then RealityKit uses `scale` as the entire entity’s clearcoat intensity value. If you provide a color image for `texture` rather than a grayscale image, RealityKit only uses the intensity of the image’s red channel.

## See Also

### Creating a clearcoat object

init(floatLiteral: Float)

Creates a clearcoat object using a single value.

init(CustomMaterial.Clearcoat)

Creates a clearcoat object from a custom material’s clearcoat property.


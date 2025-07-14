

- RealityKit
- PhysicallyBasedMaterial
- PhysicallyBasedMaterial.AnisotropyAngle
-  init(scale:texture:) 

Initializer

# init(scale:texture:)

Creates an anisotropy angle object using a single value or a texture.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+visionOS

``` source
init(
    scale: Float = 1.0,
    texture: PhysicallyBasedMaterial.Texture? = nil
)
```

## Parameters 

`scale`  

The anisotropy angle value for the entire material.

`texture`  

The anisotropy angle values as a UV-mapped image.

## Discussion

This initializer allows you to create an instance using either a single value for the entire material, or a UV-mapped image.

If you specify `texture`, RealityKit calculates the anisotropy angle for the entity by UV-mapping `texture` onto the entity and multiplying the value of each mapped pixel by `scale`. If you don’t specify `texture`, then RealityKit uses `scale` as the entire entity’s anisotropy angle. If you provide a color image for `texture` rather than a grayscale image, RealityKit only uses the intensity of the image’s red channel.

## See Also

### Creating an anisotropy angle object

init(floatLiteral: Float)

Creates an anisotropy angle object from a single value.


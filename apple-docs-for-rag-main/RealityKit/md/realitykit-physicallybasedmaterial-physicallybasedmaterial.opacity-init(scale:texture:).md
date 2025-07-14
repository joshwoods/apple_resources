

- RealityKit
- PhysicallyBasedMaterial
- PhysicallyBasedMaterial.Opacity
-  init(scale:texture:) 

Initializer

# init(scale:texture:)

Creates an opacity object using a single value or a texture.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+visionOS

``` source
init(
    scale: Float = 1.0,
    texture: PhysicallyBasedMaterial.Texture? = nil
)
```

## Parameters 

`scale`  

The opacity value for the entire material.

`texture`  

The opacity values as a UV-mapped image.

## Discussion

This initializer allows you to create an instance using either a single value for the entire material or a UV-mapped image. If `texture` is non-`nil`, RealityKit uses that image to determine the material’s opacity and ignores `scale`. If `texture` is `nil`, then it uses `scale` for the entire material.

## See Also

### Creating an opacity object

init(floatLiteral: Float)

Creates an opacity object using a single value.

init(CustomMaterial.Opacity)

Creates an opacity object using a custom material’s opacity property.




- RealityKit
- CustomMaterial
- CustomMaterial.EmissiveColor
-  init(color:texture:) 

Initializer

# init(color:texture:)

Creates a color of emitted light in macOS.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+

``` source
init(
    color: UIColor = .black,
    texture: CustomMaterial.Texture? = nil
)
```

## Parameters 

`color`  

The color of the emitted light. Defaults to black.

`texture`  

An optional UV-mapped image texture.

## See Also

### Creating an emissive color object

init(PhysicallyBasedMaterial.EmissiveColor)

Creates a color of emitted light based on the emissive color property from a physically based material.

init(color: NSColor, texture: CustomMaterial.Texture?)

Creates a color of emitted light in macOS.


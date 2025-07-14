

- RealityKit
- UnlitMaterial
-  init(color:) 

Initializer

# init(color:)

Creates an unlit material with the given base color.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+

``` source
init(color: NSColor)
```

## Parameters 

`color`  

The base color for the new material.

## Discussion

Note

The blending mode of `UnlitMaterial` materials should be configured explicitly with the blending property for transparent or translucent surfaces. The `opaque` mode is used when unset.

## See Also

### Creating an unlit material

init()

Creates an unlit material.

init(color: UIColor)

Creates an unlit material with the given base color.

init(applyPostProcessToneMap: Bool)

init(color: NSColor, applyPostProcessToneMap: Bool)

init(color: UIColor, applyPostProcessToneMap: Bool)

init(program: UnlitMaterial.Program)

init(texture: TextureResource)

Creates a new unlit material with the provided color texture.


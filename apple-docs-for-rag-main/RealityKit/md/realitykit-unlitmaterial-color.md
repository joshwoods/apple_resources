

- RealityKit
- UnlitMaterial
-  color 

Instance Property

# color

The material’s base color.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+visionOS

``` source
var color: UnlitMaterial.BaseColor { get set }
```

## Discussion

Note

The blending mode of `UnlitMaterial` materials should be configured explicitly with the blending property for transparent or translucent surfaces. The `opaque` mode is used when unset.

## See Also

### Configuring base color

var baseColor: MaterialColorParameter

The base color of the material.

Deprecated


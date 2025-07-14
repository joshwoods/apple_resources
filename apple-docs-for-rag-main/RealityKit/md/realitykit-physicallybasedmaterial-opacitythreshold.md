

- RealityKit
- PhysicallyBasedMaterial
-  opacityThreshold 

Instance Property

# opacityThreshold

A threshold below which RealityKit ignores opacity.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+visionOS

``` source
var opacityThreshold: Float? { get set }
```

## Mentioned in 

Applying realistic material and lighting effects to entities

## Discussion

When `opacityThreshold` is set, RealityKit discards pixels with opacity values less than the `opacityThreshold`, and renders opacity values greater than or equal to `opacityThreshold` fully opaque.

Note

When the `opacityThreshold` property is set, the blend mode of the blending property is ignored and the renderer applies the masking behavior.

## See Also

### Specifying opacity

case opaque

An opaque surface.

case transparent(opacity: PhysicallyBasedMaterial.Opacity)

A surface that’s transparent.

struct Opacity

An object that defines the opacity of an entity.


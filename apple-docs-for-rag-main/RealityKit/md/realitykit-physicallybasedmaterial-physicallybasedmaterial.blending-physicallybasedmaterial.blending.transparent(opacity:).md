

- RealityKit
- PhysicallyBasedMaterial
- PhysicallyBasedMaterial.Blending
-  PhysicallyBasedMaterial.Blending.transparent(opacity:) 

Case

# PhysicallyBasedMaterial.Blending.transparent(opacity:)

A surface that’s transparent.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+visionOS

``` source
case transparent(opacity: PhysicallyBasedMaterial.Opacity)
```

## Parameters 

`opacity`  

The opacity of the material.

## Discussion

This enumeration case indicates that the material supports transparency.

## See Also

### Specifying opacity

case opaque

An opaque surface.

var opacityThreshold: Float?

A threshold below which RealityKit ignores opacity.

struct Opacity

An object that defines the opacity of an entity.


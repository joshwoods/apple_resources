

- RealityKit
- PhysicallyBasedMaterial
- PhysicallyBasedMaterial.Opacity
-  PhysicallyBasedMaterial.Opacity.FloatLiteralType 

Type Alias

# PhysicallyBasedMaterial.Opacity.FloatLiteralType

A type that represents a floating-point literal.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+visionOS

``` source
typealias FloatLiteralType = Float
```

## Discussion

Valid types for `FloatLiteralType` are `Float`, `Double`, and `Float80` where available.

## See Also

### Accessing opacity values

var texture: PhysicallyBasedMaterial.Texture?

The amount of opacity specified using a UV-mapped image.

static var textureSemantic: TextureResource.Semantic

The intended use of the object’s texture property.

var scale: Float

var opacityThreshold: Float?

A threshold below which RealityKit ignores opacity.


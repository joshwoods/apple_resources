

- RealityKit
- PhysicallyBasedMaterial
- PhysicallyBasedMaterial.AnisotropyLevel
-  PhysicallyBasedMaterial.AnisotropyLevel.FloatLiteralType 

Type Alias

# PhysicallyBasedMaterial.AnisotropyLevel.FloatLiteralType

A type that represents a floating-point literal.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+visionOS

``` source
typealias FloatLiteralType = Float
```

## Discussion

Valid types for `FloatLiteralType` are `Float`, `Double`, and `Float80` where available.

## See Also

### Accessing anisotropy level values

var texture: PhysicallyBasedMaterial.Texture?

The anisotropy level values specified using a UV-mapped image.

static let textureSemantic: TextureResource.Semantic

The intended use of the object’s texture property.

var scale: Float

The anistropy level specified as a single value.


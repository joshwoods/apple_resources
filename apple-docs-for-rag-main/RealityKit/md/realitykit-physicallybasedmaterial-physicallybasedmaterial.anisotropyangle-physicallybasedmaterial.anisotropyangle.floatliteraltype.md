

- RealityKit
- PhysicallyBasedMaterial
- PhysicallyBasedMaterial.AnisotropyAngle
-  PhysicallyBasedMaterial.AnisotropyAngle.FloatLiteralType 

Type Alias

# PhysicallyBasedMaterial.AnisotropyAngle.FloatLiteralType

A type that represents a floating-point literal.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+visionOS

``` source
typealias FloatLiteralType = Float
```

## Discussion

Valid types for `FloatLiteralType` are `Float`, `Double`, and `Float80` where available.

## See Also

### Accessing anisotropy angle values

var texture: PhysicallyBasedMaterial.Texture?

The anisotropy angle values specified using a UV-mapped image.

static let textureSemantic: TextureResource.Semantic

The intended use of the object’s texture property.

var scale: Float

The anistropy angle specified as a single value.




- RealityKit
- PhysicallyBasedMaterial
- PhysicallyBasedMaterial.Metallic
-  PhysicallyBasedMaterial.Metallic.FloatLiteralType 

Type Alias

# PhysicallyBasedMaterial.Metallic.FloatLiteralType

A type that represents a floating-point literal.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+visionOS

``` source
typealias FloatLiteralType = Float
```

## Discussion

Valid types for `FloatLiteralType` are `Float`, `Double`, and `Float80` where available.

## See Also

### Accessing metallic data

var texture: PhysicallyBasedMaterial.Texture?

The reflectiveness as a UV-mapped image texture.

static let textureSemantic: TextureResource.Semantic

The intended use of the object’s texture property.

var scale: Float

The reflectiveness for the entire entity.


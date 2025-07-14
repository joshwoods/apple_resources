

- RealityKit
- PhysicallyBasedMaterial
- PhysicallyBasedMaterial.Clearcoat
-  PhysicallyBasedMaterial.Clearcoat.FloatLiteralType 

Type Alias

# PhysicallyBasedMaterial.Clearcoat.FloatLiteralType

A type that represents a floating-point literal.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+visionOS

``` source
typealias FloatLiteralType = Float
```

## Discussion

Valid types for `FloatLiteralType` are `Float`, `Double`, and `Float80` where available.

## See Also

### Accessing clearcoat values

var texture: PhysicallyBasedMaterial.Texture?

The clearcoat intensity specified using a UV-mapped image.

static let textureSemantic: TextureResource.Semantic

The intended use of the object’s texture property.

var scale: Float

The clearcoat intensity specified as a single value.


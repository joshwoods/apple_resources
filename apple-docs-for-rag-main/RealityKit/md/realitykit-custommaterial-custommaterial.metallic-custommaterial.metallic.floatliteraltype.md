

- RealityKit
- CustomMaterial
- CustomMaterial.Metallic
-  CustomMaterial.Metallic.FloatLiteralType 

Type Alias

# CustomMaterial.Metallic.FloatLiteralType

A type that represents a floating-point literal.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+

``` source
typealias FloatLiteralType = Float
```

## Discussion

Valid types for `FloatLiteralType` are `Float`, `Double`, and `Float80` where available.

## See Also

### Accessing metallic data

var scale: Float

The reflectiveness value for the entire entity or a multiplier for the metallic texture.

var texture: CustomMaterial.Texture?

The reflectiveness as a UV-mapped image texture.


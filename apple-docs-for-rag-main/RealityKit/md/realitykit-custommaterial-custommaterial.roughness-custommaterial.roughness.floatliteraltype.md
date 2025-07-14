

- RealityKit
- CustomMaterial
- CustomMaterial.Roughness
-  CustomMaterial.Roughness.FloatLiteralType 

Type Alias

# CustomMaterial.Roughness.FloatLiteralType

A type that represents a floating-point literal.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+

``` source
typealias FloatLiteralType = Float
```

## Discussion

Valid types for `FloatLiteralType` are `Float`, `Double`, and `Float80` where available.

## See Also

### Accessing roughness values

var scale: Float

The roughness value for the entire entity or a multiplier for its texture.

var texture: CustomMaterial.Texture?

The roughness values as a UV-mapped image texture.


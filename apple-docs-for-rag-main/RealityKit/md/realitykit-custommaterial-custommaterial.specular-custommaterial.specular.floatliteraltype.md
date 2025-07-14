

- RealityKit
- CustomMaterial
- CustomMaterial.Specular
-  CustomMaterial.Specular.FloatLiteralType 

Type Alias

# CustomMaterial.Specular.FloatLiteralType

A type that represents a floating-point literal.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+

``` source
typealias FloatLiteralType = Float
```

## Discussion

Valid types for `FloatLiteralType` are `Float`, `Double`, and `Float80` where available.

## See Also

### Accessing specular values

var scale: Float

The specular value for the entire entity or a multiplier for values sampled from the material’s texture.

var texture: CustomMaterial.Texture?

The specular value as a UV-mapped image texture.


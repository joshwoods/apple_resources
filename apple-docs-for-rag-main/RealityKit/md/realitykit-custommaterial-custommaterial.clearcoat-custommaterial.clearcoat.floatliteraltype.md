

- RealityKit
- CustomMaterial
- CustomMaterial.Clearcoat
-  CustomMaterial.Clearcoat.FloatLiteralType 

Type Alias

# CustomMaterial.Clearcoat.FloatLiteralType

A type that represents a floating-point literal.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+

``` source
typealias FloatLiteralType = Float
```

## Discussion

Valid types for `FloatLiteralType` are `Float`, `Double`, and `Float80` where available.

## See Also

### Accessing clearcoat values

var scale: Float

The intensity of the clearcoat.

var texture: CustomMaterial.Texture?

The clearcoat intensity specified using a UV-mapped image.


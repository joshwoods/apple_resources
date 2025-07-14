

- RealityKit
- CustomMaterial
- CustomMaterial.Clearcoat
-  scale 

Instance Property

# scale

The intensity of the clearcoat.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+

``` source
var scale: Float
```

## Discussion

Use the scale value either to hold a uniform clearcoat value that applies to the entire entity, or use it as a multiplier to scale the clearcoat intensity sampled from the texture property.

## See Also

### Accessing clearcoat values

var texture: CustomMaterial.Texture?

The clearcoat intensity specified using a UV-mapped image.

typealias FloatLiteralType

A type that represents a floating-point literal.


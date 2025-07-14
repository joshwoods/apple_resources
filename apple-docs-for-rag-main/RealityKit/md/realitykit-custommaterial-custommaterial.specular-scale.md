

- RealityKit
- CustomMaterial
- CustomMaterial.Specular
-  scale 

Instance Property

# scale

The specular value for the entire entity or a multiplier for values sampled from the material’s texture.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+

``` source
var scale: Float
```

## Discussion

If texture is `nil`, RealityKit uses this value for the opacity of the entire material. If texture isn’t `nil`, RealityKit multiplies the value sampled from texture by this property to calculate the final opacity values.

## See Also

### Accessing specular values

var texture: CustomMaterial.Texture?

The specular value as a UV-mapped image texture.

typealias FloatLiteralType

A type that represents a floating-point literal.


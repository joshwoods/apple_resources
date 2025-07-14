

- RealityKit
- CustomMaterial
- CustomMaterial.Opacity
-  scale 

Instance Property

# scale

The amount of opacity specified as a single value.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+

``` source
var scale: Float
```

## Discussion

If texture is `nil`, RealityKit uses this value for the opacity of the entire material. If texture isn’t `nil`, RealityKit multiplies the value sampled from texture by this property to calculate the final opacity values.

## See Also

### Accessing opacity data

var texture: CustomMaterial.Texture?

The amount of opacity specified using a UV-mapped image.

typealias FloatLiteralType

A type that represents a floating-point literal.


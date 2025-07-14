

- RealityKit
- CustomMaterial
- CustomMaterial.Metallic
-  scale 

Instance Property

# scale

The reflectiveness value for the entire entity or a multiplier for the metallic texture.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+

``` source
var scale: Float
```

## Discussion

This property is an input to your material’s surface shader. Although you can choose how to use the `scale` value in your shader, RealityKit provides this property to control the reflectiveness of the entire entity when there’s no texture, or to function as a multiplier to the values you sample from the texture.

## See Also

### Accessing metallic data

var texture: CustomMaterial.Texture?

The reflectiveness as a UV-mapped image texture.

typealias FloatLiteralType

A type that represents a floating-point literal.


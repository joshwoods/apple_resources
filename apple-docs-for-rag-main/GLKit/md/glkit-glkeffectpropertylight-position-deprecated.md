

- GLKit
- GLKEffectPropertyLight
-  position Deprecated

Instance Property

# position

The position of the light in world coordinates.

iOS 5.0–12.0DeprecatediPadOS 5.0–12.0DeprecatedmacOS 10.8–10.14DeprecatedtvOS 9.0–12.0Deprecated

``` source
var position: GLKVector4 { get set }
```

Deprecated

OpenGLES API deprecated. (Define GLES_SILENCE_DEPRECATION to silence these warnings)

## Discussion

If the `w` component of the position is `0.0`, the light is calculated using the directional light formula. The `x`, `y`, and `z` components of the vector specify the direction the light shines. The light is assumed to be infinitely far away; attenuation and spotlight properties are ignored.

If the `w` component of the position is a non-zero value, the coordinates specify the position of the light in homogenous coordinates, and the light is either calculated as a point light or a spotlight, depending on the value of the spotCutoff property.

The default value is `[0.0, 0.0, 1.0, 0.0]`.

## See Also

### Configuring Common Lighting Properties

var enabled: GLboolean

A Boolean value that indicates whether calculations should be performed on this light.

Deprecated

var transform: GLKEffectPropertyTransform

A transform applied to the light’s position and direction before calculating the contribution of the light.

Deprecated




- GLKit
- GLKEffectPropertyLight
-  enabled Deprecated

Instance Property

# enabled

A Boolean value that indicates whether calculations should be performed on this light.

iOS 5.0–12.0DeprecatediPadOS 5.0–12.0DeprecatedmacOS 10.8–10.14DeprecatedtvOS 9.0–12.0Deprecated

``` source
var enabled: GLboolean { get set }
```

Deprecated

OpenGLES API deprecated. (Define GLES_SILENCE_DEPRECATION to silence these warnings)

## Discussion

If the value of enabled is `GL_TRUE`, then lighting calculations are performed for this light. If the value is `GL_FALSE`, this light is skipped when computing the fragment color.

## See Also

### Configuring Common Lighting Properties

var position: GLKVector4

The position of the light in world coordinates.

Deprecated

var transform: GLKEffectPropertyTransform

A transform applied to the light’s position and direction before calculating the contribution of the light.

Deprecated


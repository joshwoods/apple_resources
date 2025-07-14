

- GLKit
- GLKEffectPropertyLight
-  transform Deprecated

Instance Property

# transform

A transform applied to the light’s position and direction before calculating the contribution of the light.

iOS 5.0–12.0DeprecatediPadOS 5.0–12.0DeprecatedmacOS 10.8–10.14DeprecatedtvOS 9.0–12.0Deprecated

``` source
var transform: GLKEffectPropertyTransform { get set }
```

Deprecated

OpenGLES API deprecated. (Define GLES_SILENCE_DEPRECATION to silence these warnings)

## Discussion

The default value is the identity matrix.

## See Also

### Configuring Common Lighting Properties

var enabled: GLboolean

A Boolean value that indicates whether calculations should be performed on this light.

Deprecated

var position: GLKVector4

The position of the light in world coordinates.

Deprecated


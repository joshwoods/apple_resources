

- GLKit
- GLKEffectPropertyFog
-  density Deprecated

Instance Property

# density

The rate at which the fog exponent increases.

iOS 5.0–12.0DeprecatediPadOS 5.0–12.0DeprecatedmacOS 10.8–10.14DeprecatedtvOS 9.0–12.0Deprecated

``` source
var density: GLfloat { get set }
```

Deprecated

OpenGLES API deprecated. (Define GLES_SILENCE_DEPRECATION to silence these warnings)

## Discussion

This property is ignored when the mode property is set to GLKFogMode.linear.

## See Also

### Fog Properties

var color: GLKVector4

The color of the fog at maximum density.

Deprecated

var start: GLfloat

The minimum distance in eye coordinates before fog is applied to the fragment color.

Deprecated

var end: GLfloat

The distance in eye coordinates where fog completely covers the color fragment.

Deprecated


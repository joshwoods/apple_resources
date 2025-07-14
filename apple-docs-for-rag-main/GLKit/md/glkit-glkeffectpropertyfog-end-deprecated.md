

- GLKit
- GLKEffectPropertyFog
-  end Deprecated

Instance Property

# end

The distance in eye coordinates where fog completely covers the color fragment.

iOS 5.0–12.0DeprecatediPadOS 5.0–12.0DeprecatedmacOS 10.8–10.14DeprecatedtvOS 9.0–12.0Deprecated

``` source
var end: GLfloat { get set }
```

Deprecated

OpenGLES API deprecated. (Define GLES_SILENCE_DEPRECATION to silence these warnings)

## Discussion

This property is ignored when the mode property is set to GLKFogMode.exp or GLKFogMode.exp2.

## See Also

### Fog Properties

var color: GLKVector4

The color of the fog at maximum density.

Deprecated

var density: GLfloat

The rate at which the fog exponent increases.

Deprecated

var start: GLfloat

The minimum distance in eye coordinates before fog is applied to the fragment color.

Deprecated


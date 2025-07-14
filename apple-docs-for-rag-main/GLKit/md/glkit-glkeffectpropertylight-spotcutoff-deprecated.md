

- GLKit
- GLKEffectPropertyLight
-  spotCutoff Deprecated

Instance Property

# spotCutoff

The angle in degrees where the spotlight is cut off.

iOS 5.0–12.0DeprecatediPadOS 5.0–12.0DeprecatedmacOS 10.8–10.14DeprecatedtvOS 9.0–12.0Deprecated

``` source
var spotCutoff: GLfloat { get set }
```

Deprecated

OpenGLES API deprecated. (Define GLES_SILENCE_DEPRECATION to silence these warnings)

## Discussion

If the `w` component of the position is not equal to `0.0`, the value of the spotCutoff property determines whether the light is a point light or a spotlight. A cutoff value of `180.0` indicates that the light is a point light; for a point light, the spotDirection and spotExponent properties are ignored. Otherwise, the spotCutoff property represents the maximum angle at which the light contributes lighting to the scene. The angle is measured between the vector provided by the spotDirection property and a vector drawn from the light’s position to the point being lit. If the angle exceeds this amount, then the light contributes no light to the scene.

The default value is `180.0`.

## See Also

### Configuring Spotlight Properties

var spotDirection: GLKVector3

A vector indicating the direction the spotlight is projecting.

Deprecated

var spotExponent: GLfloat

A value indicating how focused the spotlight is.

Deprecated


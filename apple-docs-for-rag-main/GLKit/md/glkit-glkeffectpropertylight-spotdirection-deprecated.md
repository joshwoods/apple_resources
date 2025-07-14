

- GLKit
- GLKEffectPropertyLight
-  spotDirection Deprecated

Instance Property

# spotDirection

A vector indicating the direction the spotlight is projecting.

iOS 5.0–12.0DeprecatediPadOS 5.0–12.0DeprecatedmacOS 10.8–10.14DeprecatedtvOS 9.0–12.0Deprecated

``` source
var spotDirection: GLKVector3 { get set }
```

Deprecated

OpenGLES API deprecated. (Define GLES_SILENCE_DEPRECATION to silence these warnings)

## Discussion

The default direction is `[0.0, 0.0, -1.0]`.

## See Also

### Configuring Spotlight Properties

var spotCutoff: GLfloat

The angle in degrees where the spotlight is cut off.

Deprecated

var spotExponent: GLfloat

A value indicating how focused the spotlight is.

Deprecated


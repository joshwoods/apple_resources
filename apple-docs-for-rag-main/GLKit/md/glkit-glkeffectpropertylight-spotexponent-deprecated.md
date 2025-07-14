

- GLKit
- GLKEffectPropertyLight
-  spotExponent Deprecated

Instance Property

# spotExponent

A value indicating how focused the spotlight is.

iOS 5.0–12.0DeprecatediPadOS 5.0–12.0DeprecatedmacOS 10.8–10.14DeprecatedtvOS 9.0–12.0Deprecated

``` source
var spotExponent: GLfloat { get set }
```

Deprecated

OpenGLES API deprecated. (Define GLES_SILENCE_DEPRECATION to silence these warnings)

## Discussion

The higher the value stored in the spotExponent property, the tighter the focus of the spotlight. The default value is `0.0`.

## See Also

### Configuring Spotlight Properties

var spotCutoff: GLfloat

The angle in degrees where the spotlight is cut off.

Deprecated

var spotDirection: GLKVector3

A vector indicating the direction the spotlight is projecting.

Deprecated


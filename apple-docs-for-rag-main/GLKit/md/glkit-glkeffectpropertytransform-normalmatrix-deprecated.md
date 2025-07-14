

- GLKit
- GLKEffectPropertyTransform
-  normalMatrix Deprecated

Instance Property

# normalMatrix

The matrix used to transform normal coordinates from world space to eye space.

iOS 5.0–12.0DeprecatediPadOS 5.0–12.0DeprecatedmacOS 10.8–10.14DeprecatedtvOS 9.0–12.0Deprecated

``` source
var normalMatrix: GLKMatrix3 { get }
```

Deprecated

OpenGLES API deprecated. (Define GLES_SILENCE_DEPRECATION to silence these warnings)

## Discussion

The normal matrix is derived from the modelviewMatrix property and is automatically calculated when needed.

## See Also

### Configuring Modelview Properties

var modelviewMatrix: GLKMatrix4

The matrix used to transform position coordinates from world space to eye space.

Deprecated


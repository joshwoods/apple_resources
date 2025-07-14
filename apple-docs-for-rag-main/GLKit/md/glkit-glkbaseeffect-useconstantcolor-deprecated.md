

- GLKit
- GLKBaseEffect
-  useConstantColor Deprecated

Instance Property

# useConstantColor

A Boolean value that indicates whether or not to use the constant color.

iOS 5.0–12.0DeprecatediPadOS 5.0–12.0DeprecatedmacOS 10.8–10.14DeprecatedtvOS 9.0–12.0Deprecated

``` source
var useConstantColor: GLboolean { get set }
```

Deprecated

OpenGLES API deprecated. (Define GLES_SILENCE_DEPRECATION to silence these warnings)

## Discussion

If the value is set to `GL_TRUE`, then the value stored in the constantColor property is used as the color value for each vertex. If the value is set to `GL_FALSE`, then your application is expected to enable the GLKVertexAttrib.color attribute and provide per-vertex color data. The default value is `GL_FALSE`.

## See Also

### Configuring Color Information

var colorMaterialEnabled: GLboolean

A Boolean value that indicates whether or not to use the color vertex attribute when calculating the light’s interaction with the material.

Deprecated

var constantColor: GLKVector4

A constant color, used when per-vertex color data is not provided.

Deprecated


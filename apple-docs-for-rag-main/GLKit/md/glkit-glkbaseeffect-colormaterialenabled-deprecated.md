

- GLKit
- GLKBaseEffect
-  colorMaterialEnabled Deprecated

Instance Property

# colorMaterialEnabled

A Boolean value that indicates whether or not to use the color vertex attribute when calculating the light’s interaction with the material.

iOS 5.0–12.0DeprecatediPadOS 5.0–12.0DeprecatedmacOS 10.8–10.14DeprecatedtvOS 9.0–12.0Deprecated

``` source
var colorMaterialEnabled: GLboolean { get set }
```

Deprecated

OpenGLES API deprecated. (Define GLES_SILENCE_DEPRECATION to silence these warnings)

## Discussion

If the value is set to `GL_TRUE`, then the color attribute provided in the vertex data is used as the material’s color when performing any lighting calculations. If the value is set to `GL_FALSE` then the colors stored in the material property are used to light the primitive. The default value is `GL_FALSE`.

## See Also

### Configuring Color Information

var useConstantColor: GLboolean

A Boolean value that indicates whether or not to use the constant color.

Deprecated

var constantColor: GLKVector4

A constant color, used when per-vertex color data is not provided.

Deprecated


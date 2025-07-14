

- GLKit
- GLKEffectPropertyTexture
-  enabled Deprecated

Instance Property

# enabled

A Boolean value that indicates whether this texture is used to texture drawn primitives.

iOS 5.0–12.0DeprecatediPadOS 5.0–12.0DeprecatedmacOS 10.8–10.14DeprecatedtvOS 9.0–12.0Deprecated

``` source
var enabled: GLboolean { get set }
```

Deprecated

OpenGLES API deprecated. (Define GLES_SILENCE_DEPRECATION to silence these warnings)

## Discussion

If the value is `GL_TRUE`, then the texture is applied to the primitive. If the value is `GL_FALSE`, the texture is skipped. The default value is `GL_TRUE`.

## See Also

### Configuring Texture Properties

var envMode: GLKTextureEnvMode

The mode the texture uses to compute its output fragment color. See GLKTextureEnvMode.

Deprecated

var name: GLuint

The OpenGL name for the texture being sampled by this texture stage.

Deprecated

var target: GLKTextureTarget

The kind of texture pointed to by the texture stage. See GLKTextureTarget.

Deprecated


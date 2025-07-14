

- GLKit
- GLKEffectPropertyTexture
-  envMode Deprecated

Instance Property

# envMode

The mode the texture uses to compute its output fragment color. See GLKTextureEnvMode.

iOS 5.0–12.0DeprecatediPadOS 5.0–12.0DeprecatedmacOS 10.8–10.14DeprecatedtvOS 9.0–12.0Deprecated

``` source
var envMode: GLKTextureEnvMode { get set }
```

Deprecated

OpenGLES API deprecated. (Define GLES_SILENCE_DEPRECATION to silence these warnings)

## Discussion

The default value is GLKTextureEnvMode.modulate.

## See Also

### Configuring Texture Properties

var enabled: GLboolean

A Boolean value that indicates whether this texture is used to texture drawn primitives.

Deprecated

var name: GLuint

The OpenGL name for the texture being sampled by this texture stage.

Deprecated

var target: GLKTextureTarget

The kind of texture pointed to by the texture stage. See GLKTextureTarget.

Deprecated


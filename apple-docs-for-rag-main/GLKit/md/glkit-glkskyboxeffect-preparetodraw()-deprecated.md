

- GLKit
- GLKSkyboxEffect
-  prepareToDraw() Deprecated

Instance Method

# prepareToDraw()

Prepares an effect for rendering.

iOS 5.0–12.0DeprecatediPadOS 5.0–12.0DeprecatedmacOS 10.8–10.14DeprecatedtvOS 9.0–12.0Deprecated

``` source
func prepareToDraw()
```

Deprecated

OpenGLES API deprecated. (Define GLES_SILENCE_DEPRECATION to silence these warnings)

## Discussion

When the skybox shader is bound, the following state variables are altered:

- `GL_CURRENT_PROGRAM`

- `GL_TEXTURE_BINDING_CUBE_MAP`

- `GL_VERTEX_ARRAY_BINDING_OES`

- `GL_VERTEX_ATTRIB_ARRAY_ENABLED`

Your application is responsible for saving and restoring these variables, if necessary for it to execute correctly.


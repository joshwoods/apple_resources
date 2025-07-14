

- GLKit
- GLKBaseEffect
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

An effect must be prepared after it is configured and again when your application wants to use the effect to render any primitives. When your application prepares an effect, some OpenGL state is altered to allow the effect to operate:

- The `GL_CURRENT_PROGRAM` state is always changed to point to the shader provided by the effect object.

- When texturing is enabled, the `GL_TEXTURE_BINDING_2D` state may also change.

If your application requires the previous state to be saved before the effect alters them, it must explicitly save and restore the values.


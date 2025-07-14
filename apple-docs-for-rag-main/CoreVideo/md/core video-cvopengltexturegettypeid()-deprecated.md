

- Core Video
-  CVOpenGLTextureGetTypeID() Deprecated

Function

# CVOpenGLTextureGetTypeID()

Obtains the Core Foundation ID for the Core Video OpenGL texture type.

macOS 10.4–10.14Deprecated

``` source
func CVOpenGLTextureGetTypeID() -> CFTypeID
```

Deprecated

OpenGL/OpenGLES is no longer supported. Use Metal APIs instead. (Define COREVIDEO_SILENCE_GL_DEPRECATION to silence these warnings)

## Return Value

The Core Foundation ID for this type.

## See Also

### Inspecting Textures

func CVOpenGLTextureGetName(CVOpenGLTexture) -> GLuint

Returns the texture target name of a CoreVideo OpenGL texture.

Deprecated

func CVOpenGLTextureGetTarget(CVOpenGLTexture) -> GLenum

Returns the texture target (for example, `GL_TEXTURE_2D`) of an OpenGL texture.

Deprecated

func CVOpenGLTextureGetCleanTexCoords(CVOpenGLTexture, UnsafeMutablePointer&lt;GLfloat>, UnsafeMutablePointer&lt;GLfloat>, UnsafeMutablePointer&lt;GLfloat>, UnsafeMutablePointer&lt;GLfloat>)

Returns the texture coordinates for the part of the image that should be displayed.

Deprecated

func CVOpenGLTextureIsFlipped(CVOpenGLTexture) -> Bool

Determines whether an OpenGL texture is flipped vertically.

Deprecated


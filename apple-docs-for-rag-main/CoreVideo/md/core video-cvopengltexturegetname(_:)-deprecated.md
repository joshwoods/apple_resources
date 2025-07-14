

- Core Video
-  CVOpenGLTextureGetName(\_:) Deprecated

Function

# CVOpenGLTextureGetName(\_:)

Returns the texture target name of a CoreVideo OpenGL texture.

macOS 10.4–10.14Deprecated

``` source
func CVOpenGLTextureGetName(_ image: CVOpenGLTexture) -> GLuint
```

Deprecated

OpenGL/OpenGLES is no longer supported. Use Metal APIs instead. (Define COREVIDEO_SILENCE_GL_DEPRECATION to silence these warnings)

## Parameters 

`image`  

The Core Video OpenGL texture whose texture target name you want to obtain.

## Return Value

The target name of the texture.

## Discussion

See the OpenGL specification for more information about texture targets.

## See Also

### Inspecting Textures

func CVOpenGLTextureGetTarget(CVOpenGLTexture) -> GLenum

Returns the texture target (for example, `GL_TEXTURE_2D`) of an OpenGL texture.

Deprecated

func CVOpenGLTextureGetCleanTexCoords(CVOpenGLTexture, UnsafeMutablePointer&lt;GLfloat>, UnsafeMutablePointer&lt;GLfloat>, UnsafeMutablePointer&lt;GLfloat>, UnsafeMutablePointer&lt;GLfloat>)

Returns the texture coordinates for the part of the image that should be displayed.

Deprecated

func CVOpenGLTextureIsFlipped(CVOpenGLTexture) -> Bool

Determines whether an OpenGL texture is flipped vertically.

Deprecated

func CVOpenGLTextureGetTypeID() -> CFTypeID

Obtains the Core Foundation ID for the Core Video OpenGL texture type.

Deprecated


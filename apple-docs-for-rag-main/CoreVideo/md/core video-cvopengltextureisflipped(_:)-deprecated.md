

- Core Video
-  CVOpenGLTextureIsFlipped(\_:) Deprecated

Function

# CVOpenGLTextureIsFlipped(\_:)

Determines whether an OpenGL texture is flipped vertically.

macOS 10.4–10.14Deprecated

``` source
func CVOpenGLTextureIsFlipped(_ image: CVOpenGLTexture) -> Bool
```

Deprecated

OpenGL/OpenGLES is no longer supported. Use Metal APIs instead. (Define COREVIDEO_SILENCE_GL_DEPRECATION to silence these warnings)

## Parameters 

`image`  

The Core Video OpenGL texture whose vertical orientation you want to determine.

## Return Value

Returns `true` if (0,0) in the texture is in the upper-left corner, and `false` if (0,0) is in the lower-left corner.

## Discussion

Quartz assumes a lower-left origin.

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

func CVOpenGLTextureGetTypeID() -> CFTypeID

Obtains the Core Foundation ID for the Core Video OpenGL texture type.

Deprecated


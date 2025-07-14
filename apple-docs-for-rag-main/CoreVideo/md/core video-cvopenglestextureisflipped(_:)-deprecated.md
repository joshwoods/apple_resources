

- Core Video
-  CVOpenGLESTextureIsFlipped(\_:) Deprecated

Function

# CVOpenGLESTextureIsFlipped(\_:)

Returns whether the image is flipped vertically or not.

iOS 5.0–12.0DeprecatediPadOS 5.0–12.0DeprecatedtvOS 9.0–12.0Deprecated

``` source
func CVOpenGLESTextureIsFlipped(_ image: CVOpenGLESTexture) -> Bool
```

Deprecated

OpenGL/OpenGLES is no longer supported. Use Metal APIs instead. (Define COREVIDEO_SILENCE_GL_DEPRECATION to silence these warnings)

## Parameters 

`image`  

The OpenGLES texture-based image buffer whose orientation is desired.

## Return Value

`True` if `{0,0}` represents the upper left of the texture; otherwise `False` if `{0,0}` represents the lower left of the texture.

## See Also

### Inspecting Textures

func CVOpenGLESTextureGetTarget(CVOpenGLESTexture) -> GLenum

Returns the texture target for a `CVOpenGLESTextureRef`.

Deprecated

func CVOpenGLESTextureGetName(CVOpenGLESTexture) -> GLuint

Returns the texture target name for a `CVOpenGLESTextureRef`.

Deprecated

func CVOpenGLESTextureGetCleanTexCoords(CVOpenGLESTexture, UnsafeMutablePointer&lt;GLfloat>, UnsafeMutablePointer&lt;GLfloat>, UnsafeMutablePointer&lt;GLfloat>, UnsafeMutablePointer&lt;GLfloat>)

Returns convenient normalized texture coordinates for the part of the image that should be displayed.

Deprecated

func CVOpenGLESTextureGetTypeID() -> CFTypeID

Returns the Core Foundation type identifier for a Core Video texture-based image buffer.

Deprecated


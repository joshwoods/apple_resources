

- Core Video
-  CVOpenGLESTextureGetTypeID() Deprecated

Function

# CVOpenGLESTextureGetTypeID()

Returns the Core Foundation type identifier for a Core Video texture-based image buffer.

iOS 5.0–12.0DeprecatediPadOS 5.0–12.0DeprecatedtvOS 9.0–12.0Deprecated

``` source
func CVOpenGLESTextureGetTypeID() -> CFTypeID
```

Deprecated

OpenGL/OpenGLES is no longer supported. Use Metal APIs instead. (Define COREVIDEO_SILENCE_GL_DEPRECATION to silence these warnings)

## Return Value

The Core Foundation type identifier for the `CVOpenGLESTextureRef` type.

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

func CVOpenGLESTextureIsFlipped(CVOpenGLESTexture) -> Bool

Returns whether the image is flipped vertically or not.

Deprecated


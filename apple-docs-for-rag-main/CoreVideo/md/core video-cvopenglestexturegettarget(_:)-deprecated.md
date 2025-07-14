

- Core Video
-  CVOpenGLESTextureGetTarget(\_:) Deprecated

Function

# CVOpenGLESTextureGetTarget(\_:)

Returns the texture target for a `CVOpenGLESTextureRef`.

iOS 5.0–12.0DeprecatediPadOS 5.0–12.0DeprecatedtvOS 9.0–12.0Deprecated

``` source
func CVOpenGLESTextureGetTarget(_ image: CVOpenGLESTexture) -> GLenum
```

Deprecated

OpenGL/OpenGLES is no longer supported. Use Metal APIs instead. (Define COREVIDEO_SILENCE_GL_DEPRECATION to silence these warnings)

## Parameters 

`image`  

The OpenGLES texture-based image buffer whose target is desired.

## Return Value

An OpenGLES texture target, such as `GL_TEXTURE_2D`.

## See Also

### Inspecting Textures

func CVOpenGLESTextureGetName(CVOpenGLESTexture) -> GLuint

Returns the texture target name for a `CVOpenGLESTextureRef`.

Deprecated

func CVOpenGLESTextureGetCleanTexCoords(CVOpenGLESTexture, UnsafeMutablePointer&lt;GLfloat>, UnsafeMutablePointer&lt;GLfloat>, UnsafeMutablePointer&lt;GLfloat>, UnsafeMutablePointer&lt;GLfloat>)

Returns convenient normalized texture coordinates for the part of the image that should be displayed.

Deprecated

func CVOpenGLESTextureIsFlipped(CVOpenGLESTexture) -> Bool

Returns whether the image is flipped vertically or not.

Deprecated

func CVOpenGLESTextureGetTypeID() -> CFTypeID

Returns the Core Foundation type identifier for a Core Video texture-based image buffer.

Deprecated




- Core Video
-  CVOpenGLESTextureGetCleanTexCoords(\_:\_:\_:\_:\_:) Deprecated

Function

# CVOpenGLESTextureGetCleanTexCoords(\_:\_:\_:\_:\_:)

Returns convenient normalized texture coordinates for the part of the image that should be displayed.

iOS 5.0–12.0DeprecatediPadOS 5.0–12.0DeprecatedtvOS 9.0–12.0Deprecated

``` source
func CVOpenGLESTextureGetCleanTexCoords(
    _ image: CVOpenGLESTexture,
    _ lowerLeft: UnsafeMutablePointer,
    _ lowerRight: UnsafeMutablePointer,
    _ upperRight: UnsafeMutablePointer,
    _ upperLeft: UnsafeMutablePointer
)
```

Deprecated

OpenGL/OpenGLES is no longer supported. Use Metal APIs instead. (Define COREVIDEO_SILENCE_GL_DEPRECATION to silence these warnings)

## Parameters 

`image`  

The OpenGLES texture-based image buffer whose normalized texture coordinates are desired.

`lowerLeft`  

An array of two `GLfloat`s where the `s` and `t` normalized texture coordinates of the lower left corner of the image will be stored.

`lowerRight`  

An array of two `GLfloat`s where the `s` and `t` normalized texture coordinates of the lower right corner of the image will be stored.

`upperRight`  

An array of two `GLfloat`s where the `s` and `t` normalized texture coordinates of the upper right corner of the image will be stored.

`upperLeft`  

An array of two `GLfloat`s where the `s` and `t` normalized texture coordinates of the upper left corner of the image will be stored.

## Discussion

This function automatically takes into account whether or not the texture is flipped.

## See Also

### Inspecting Textures

func CVOpenGLESTextureGetTarget(CVOpenGLESTexture) -> GLenum

Returns the texture target for a `CVOpenGLESTextureRef`.

Deprecated

func CVOpenGLESTextureGetName(CVOpenGLESTexture) -> GLuint

Returns the texture target name for a `CVOpenGLESTextureRef`.

Deprecated

func CVOpenGLESTextureIsFlipped(CVOpenGLESTexture) -> Bool

Returns whether the image is flipped vertically or not.

Deprecated

func CVOpenGLESTextureGetTypeID() -> CFTypeID

Returns the Core Foundation type identifier for a Core Video texture-based image buffer.

Deprecated




- Core Video
-  CVOpenGLTextureGetCleanTexCoords(\_:\_:\_:\_:\_:) Deprecated

Function

# CVOpenGLTextureGetCleanTexCoords(\_:\_:\_:\_:\_:)

Returns the texture coordinates for the part of the image that should be displayed.

macOS 10.4–10.14Deprecated

``` source
func CVOpenGLTextureGetCleanTexCoords(
    _ image: CVOpenGLTexture,
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

The Core Video OpenGL texture whose clean tex coordinates you want to obtain.

`lowerLeft`  

On output, the `GLFloat` array holds the *s* and *t* texture coordinates of the lower-left corner of the image.

`lowerRight`  

On output, the `GLFloat` array holds the *s* and *t* texture coordinates of the lower-right corner of the image.

`upperRight`  

On output, the `GLFloat` array holds the *s* and *t* texture coordinates of the upper-right corner of the image.

`upperLeft`  

On output, the `GLFloat` array holds the *s* and *t* texture coordinates of the upper-left corner of the image.

## Discussion

This function automatically takes into account whether or not the texture is flipped.

## See Also

### Related Documentation

Core Video Programming Guide

### Inspecting Textures

func CVOpenGLTextureGetName(CVOpenGLTexture) -> GLuint

Returns the texture target name of a CoreVideo OpenGL texture.

Deprecated

func CVOpenGLTextureGetTarget(CVOpenGLTexture) -> GLenum

Returns the texture target (for example, `GL_TEXTURE_2D`) of an OpenGL texture.

Deprecated

func CVOpenGLTextureIsFlipped(CVOpenGLTexture) -> Bool

Determines whether an OpenGL texture is flipped vertically.

Deprecated

func CVOpenGLTextureGetTypeID() -> CFTypeID

Obtains the Core Foundation ID for the Core Video OpenGL texture type.

Deprecated


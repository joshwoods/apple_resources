

- Core Video
-  CVOpenGLBufferCreate(\_:\_:\_:\_:\_:) Deprecated

Function

# CVOpenGLBufferCreate(\_:\_:\_:\_:\_:)

Creates a new Core Video OpenGL buffer that can be used for OpenGL rendering purposes

macOS 10.4–10.14Deprecated

``` source
func CVOpenGLBufferCreate(
    _ allocator: CFAllocator?,
    _ width: Int,
    _ height: Int,
    _ attributes: CFDictionary?,
    _ bufferOut: UnsafeMutablePointer
) -> CVReturn
```

Deprecated

OpenGL/OpenGLES is no longer supported. Use Metal APIs instead. (Define COREVIDEO_SILENCE_GL_DEPRECATION to silence these warnings)

## Parameters 

`allocator`  

The allocator to use to create the Core Video OpenGL buffer. Pass `NULL` to specify the default allocator.

`width`  

The width of the buffer in pixels.

`height`  

The height of the buffer in pixels.

`attributes`  

A Core Foundation dictionary containing other desired attributes of the buffer (texture target, internal format, max mipmap level, etc.). May be `NULL`. The following attribute values are assumed if you do not explicitly define them:

- `kCVOpenGLBufferTarget` = `GL_TEXTURE_RECTANGLE_EXT`

- `kCVOpenGLBufferInternalFormat` = `GL_RGBA`

- `kCVOpenGLBufferMaximumMipmapLevel` = 0

`bufferOut`  

On output, `bufferOut` points to the newly created OpenGL buffer.

## Return Value

A Core Video result code. See Core Video Constants for possible values.

## Discussion

## See Also

### Functions

func CVOpenGLBufferAttach(CVOpenGLBuffer, CGLContextObj, GLenum, GLint, GLint) -> CVReturn

Attaches an OpenGL context to a Core Video OpenGL buffer.

Deprecated

func CVOpenGLBufferGetAttributes(CVOpenGLBuffer) -> Unmanaged&lt;CFDictionary>?

Obtains the attributes of a Core Video OpenGL buffer.

Deprecated

func CVOpenGLBufferGetTypeID() -> CFTypeID

Obtains the Core Foundation type ID for the OpenGL buffer type.

Deprecated


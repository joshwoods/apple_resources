

- Core Video
-  CVOpenGLBufferGetTypeID() Deprecated

Function

# CVOpenGLBufferGetTypeID()

Obtains the Core Foundation type ID for the OpenGL buffer type.

macOS 10.4–10.14Deprecated

``` source
func CVOpenGLBufferGetTypeID() -> CFTypeID
```

Deprecated

OpenGL/OpenGLES is no longer supported. Use Metal APIs instead. (Define COREVIDEO_SILENCE_GL_DEPRECATION to silence these warnings)

## Return Value

The Core Foundation ID for this data type.

## See Also

### Functions

func CVOpenGLBufferCreate(CFAllocator?, Int, Int, CFDictionary?, UnsafeMutablePointer&lt;CVOpenGLBuffer?>) -> CVReturn

Creates a new Core Video OpenGL buffer that can be used for OpenGL rendering purposes

Deprecated

func CVOpenGLBufferAttach(CVOpenGLBuffer, CGLContextObj, GLenum, GLint, GLint) -> CVReturn

Attaches an OpenGL context to a Core Video OpenGL buffer.

Deprecated

func CVOpenGLBufferGetAttributes(CVOpenGLBuffer) -> Unmanaged&lt;CFDictionary>?

Obtains the attributes of a Core Video OpenGL buffer.

Deprecated


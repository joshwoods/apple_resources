

- Core Video
-  CVOpenGLBufferGetAttributes(\_:) Deprecated

Function

# CVOpenGLBufferGetAttributes(\_:)

Obtains the attributes of a Core Video OpenGL buffer.

macOS 10.4–10.14Deprecated

``` source
func CVOpenGLBufferGetAttributes(_ openGLBuffer: CVOpenGLBuffer) -> Unmanaged?
```

Deprecated

OpenGL/OpenGLES is no longer supported. Use Metal APIs instead. (Define COREVIDEO_SILENCE_GL_DEPRECATION to silence these warnings)

## Parameters 

`openGLBuffer`  

The OpenGL buffer whose attributes you want to obtain.

## Return Value

A Core Foundation dictionary containing the OpenGL buffer attributes, or `NULL` if no attributes exist.

## See Also

### Functions

func CVOpenGLBufferCreate(CFAllocator?, Int, Int, CFDictionary?, UnsafeMutablePointer&lt;CVOpenGLBuffer?>) -> CVReturn

Creates a new Core Video OpenGL buffer that can be used for OpenGL rendering purposes

Deprecated

func CVOpenGLBufferAttach(CVOpenGLBuffer, CGLContextObj, GLenum, GLint, GLint) -> CVReturn

Attaches an OpenGL context to a Core Video OpenGL buffer.

Deprecated

func CVOpenGLBufferGetTypeID() -> CFTypeID

Obtains the Core Foundation type ID for the OpenGL buffer type.

Deprecated


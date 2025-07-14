

- Core Video
-  CVOpenGLBufferAttach(\_:\_:\_:\_:\_:) Deprecated

Function

# CVOpenGLBufferAttach(\_:\_:\_:\_:\_:)

Attaches an OpenGL context to a Core Video OpenGL buffer.

macOS 10.4–10.14Deprecated

``` source
func CVOpenGLBufferAttach(
    _ openGLBuffer: CVOpenGLBuffer,
    _ cglContext: CGLContextObj,
    _ face: GLenum,
    _ level: GLint,
    _ screen: GLint
) -> CVReturn
```

Deprecated

OpenGL/OpenGLES is no longer supported. Use Metal APIs instead. (Define COREVIDEO_SILENCE_GL_DEPRECATION to silence these warnings)

## Parameters 

`openGLBuffer`  

The buffer you want to attach an OpenGL context to.

`cglContext`  

The OpenGL context you want to attach.

`face`  

The OpenGL face enumeration (`0` for non-cube maps.)

`level`  

The mipmap level for drawing in the OpenGL context. This value cannot exceed the maximum mipmap level for this buffer.

`screen`  

The virtual screen number you want to use for this context.

## Return Value

A Core Video result code. See Core Video Constants for possible values.

## See Also

### Related Documentation

Core Video Programming Guide

### Functions

func CVOpenGLBufferCreate(CFAllocator?, Int, Int, CFDictionary?, UnsafeMutablePointer&lt;CVOpenGLBuffer?>) -> CVReturn

Creates a new Core Video OpenGL buffer that can be used for OpenGL rendering purposes

Deprecated

func CVOpenGLBufferGetAttributes(CVOpenGLBuffer) -> Unmanaged&lt;CFDictionary>?

Obtains the attributes of a Core Video OpenGL buffer.

Deprecated

func CVOpenGLBufferGetTypeID() -> CFTypeID

Obtains the Core Foundation type ID for the OpenGL buffer type.

Deprecated


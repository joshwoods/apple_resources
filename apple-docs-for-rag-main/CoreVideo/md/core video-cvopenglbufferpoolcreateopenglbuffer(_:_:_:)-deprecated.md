

- Core Video
-  CVOpenGLBufferPoolCreateOpenGLBuffer(\_:\_:\_:) Deprecated

Function

# CVOpenGLBufferPoolCreateOpenGLBuffer(\_:\_:\_:)

Creates a new OpenGL buffer from an OpenGL buffer pool.

macOS 10.4–10.14Deprecated

``` source
func CVOpenGLBufferPoolCreateOpenGLBuffer(
    _ allocator: CFAllocator?,
    _ openGLBufferPool: CVOpenGLBufferPool,
    _ openGLBufferOut: UnsafeMutablePointer
) -> CVReturn
```

Deprecated

OpenGL/OpenGLES is no longer supported. Use Metal APIs instead. (Define COREVIDEO_SILENCE_GL_DEPRECATION to silence these warnings)

## Parameters 

`allocator`  

The allocator to use for creating the buffer. May be `NULL` to specify the default allocator.

`openGLBufferPool`  

The OpenGL buffer pool that should create the new OpenGL buffer.

`openGLBufferOut`  

On output, `OpenGLBufferOut` points to the new OpenGL buffer.

## Return Value

A Core Video result code. See Core Video Constants for possible values.

## Discussion

The function creates a new OpenGL buffer using the OpenGL buffer attributes specified in the CVOpenGLBufferPoolCreate(_:_:_:_:) call. This buffer has default attachments as specified in the `openGLBufferAttributes` parameter of CVOpenGLBufferPoolCreate(_:_:_:_:) (using either the `kCVBufferPropagatedAttachmentsKey` or `kCVBufferNonPropagatedAttachmentsKey` attributes).

## See Also

### Functions

func CVOpenGLBufferPoolCreate(CFAllocator?, CFDictionary?, CFDictionary?, UnsafeMutablePointer&lt;CVOpenGLBufferPool?>) -> CVReturn

Creates a new OpenGL buffer pool.

Deprecated

func CVOpenGLBufferPoolGetAttributes(CVOpenGLBufferPool) -> Unmanaged&lt;CFDictionary>?

Returns the pool attributes dictionary for an Open GL buffer pool.

Deprecated

func CVOpenGLBufferPoolGetOpenGLBufferAttributes(CVOpenGLBufferPool) -> Unmanaged&lt;CFDictionary>?

Returns the attributes of OpenGL buffers that will be created from a buffer pool.

Deprecated

func CVOpenGLBufferPoolGetTypeID() -> CFTypeID

Obtains the Core Foundation ID for the OpenGL buffer pool type.

Deprecated


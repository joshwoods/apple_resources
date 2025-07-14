

- Core Video
-  CVOpenGLBufferPoolCreate(\_:\_:\_:\_:) Deprecated

Function

# CVOpenGLBufferPoolCreate(\_:\_:\_:\_:)

Creates a new OpenGL buffer pool.

macOS 10.4–10.14Deprecated

``` source
func CVOpenGLBufferPoolCreate(
    _ allocator: CFAllocator?,
    _ poolAttributes: CFDictionary?,
    _ openGLBufferAttributes: CFDictionary?,
    _ poolOut: UnsafeMutablePointer
) -> CVReturn
```

Deprecated

OpenGL/OpenGLES is no longer supported. Use Metal APIs instead. (Define COREVIDEO_SILENCE_GL_DEPRECATION to silence these warnings)

## Parameters 

`allocator`  

The allocator to use for allocating this buffer pool. Pass `NULL` to specify the default allocator.

`poolAttributes`  

A Core Foundation dictionary containing the attributes to be used for the pool itself.

`openGLBufferAttributes`  

A Core Foundation dictionary containing the attributes to be used for creating new OpenGL buffers within the pool.

`poolOut`  

On output, `poolOut` points to the new OpenGL buffer pool.

## Return Value

A Core Video result code. SeeCore Video Constants for possible values.

## See Also

### Functions

func CVOpenGLBufferPoolCreateOpenGLBuffer(CFAllocator?, CVOpenGLBufferPool, UnsafeMutablePointer&lt;CVOpenGLBuffer?>) -> CVReturn

Creates a new OpenGL buffer from an OpenGL buffer pool.

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


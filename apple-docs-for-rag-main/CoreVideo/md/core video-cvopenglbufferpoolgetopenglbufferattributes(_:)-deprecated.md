

- Core Video
-  CVOpenGLBufferPoolGetOpenGLBufferAttributes(\_:) Deprecated

Function

# CVOpenGLBufferPoolGetOpenGLBufferAttributes(\_:)

Returns the attributes of OpenGL buffers that will be created from a buffer pool.

macOS 10.4–10.14Deprecated

``` source
func CVOpenGLBufferPoolGetOpenGLBufferAttributes(_ pool: CVOpenGLBufferPool) -> Unmanaged?
```

Deprecated

OpenGL/OpenGLES is no longer supported. Use Metal APIs instead. (Define COREVIDEO_SILENCE_GL_DEPRECATION to silence these warnings)

## Parameters 

`pool`  

The OpenGL buffer pool containing the attributes to be retrieved.

## Return Value

The OpenGL buffer attributes Core Foundation dictionary, or `NULL` on failure.

## Discussion

You can use this function to obtain information about the OpenGL buffers that will be created from the buffer pool.

## See Also

### Functions

func CVOpenGLBufferPoolCreate(CFAllocator?, CFDictionary?, CFDictionary?, UnsafeMutablePointer&lt;CVOpenGLBufferPool?>) -> CVReturn

Creates a new OpenGL buffer pool.

Deprecated

func CVOpenGLBufferPoolCreateOpenGLBuffer(CFAllocator?, CVOpenGLBufferPool, UnsafeMutablePointer&lt;CVOpenGLBuffer?>) -> CVReturn

Creates a new OpenGL buffer from an OpenGL buffer pool.

Deprecated

func CVOpenGLBufferPoolGetAttributes(CVOpenGLBufferPool) -> Unmanaged&lt;CFDictionary>?

Returns the pool attributes dictionary for an Open GL buffer pool.

Deprecated

func CVOpenGLBufferPoolGetTypeID() -> CFTypeID

Obtains the Core Foundation ID for the OpenGL buffer pool type.

Deprecated


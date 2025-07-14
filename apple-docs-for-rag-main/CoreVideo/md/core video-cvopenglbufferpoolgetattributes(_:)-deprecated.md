

- Core Video
-  CVOpenGLBufferPoolGetAttributes(\_:) Deprecated

Function

# CVOpenGLBufferPoolGetAttributes(\_:)

Returns the pool attributes dictionary for an Open GL buffer pool.

macOS 10.4–10.14Deprecated

``` source
func CVOpenGLBufferPoolGetAttributes(_ pool: CVOpenGLBufferPool) -> Unmanaged?
```

Deprecated

OpenGL/OpenGLES is no longer supported. Use Metal APIs instead. (Define COREVIDEO_SILENCE_GL_DEPRECATION to silence these warnings)

## Parameters 

`pool`  

The OpenGL buffer pool containing the attributes to be retrieved.

## Return Value

The buffer-pool attributes Core Foundation dictionary, or `NULL` on failure.

## See Also

### Functions

func CVOpenGLBufferPoolCreate(CFAllocator?, CFDictionary?, CFDictionary?, UnsafeMutablePointer&lt;CVOpenGLBufferPool?>) -> CVReturn

Creates a new OpenGL buffer pool.

Deprecated

func CVOpenGLBufferPoolCreateOpenGLBuffer(CFAllocator?, CVOpenGLBufferPool, UnsafeMutablePointer&lt;CVOpenGLBuffer?>) -> CVReturn

Creates a new OpenGL buffer from an OpenGL buffer pool.

Deprecated

func CVOpenGLBufferPoolGetOpenGLBufferAttributes(CVOpenGLBufferPool) -> Unmanaged&lt;CFDictionary>?

Returns the attributes of OpenGL buffers that will be created from a buffer pool.

Deprecated

func CVOpenGLBufferPoolGetTypeID() -> CFTypeID

Obtains the Core Foundation ID for the OpenGL buffer pool type.

Deprecated


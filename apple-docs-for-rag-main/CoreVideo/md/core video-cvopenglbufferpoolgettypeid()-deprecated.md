

- Core Video
-  CVOpenGLBufferPoolGetTypeID() Deprecated

Function

# CVOpenGLBufferPoolGetTypeID()

Obtains the Core Foundation ID for the OpenGL buffer pool type.

macOS 10.4–10.14Deprecated

``` source
func CVOpenGLBufferPoolGetTypeID() -> CFTypeID
```

Deprecated

OpenGL/OpenGLES is no longer supported. Use Metal APIs instead. (Define COREVIDEO_SILENCE_GL_DEPRECATION to silence these warnings)

## Return Value

The Core Foundation ID for this data type.

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

func CVOpenGLBufferPoolGetOpenGLBufferAttributes(CVOpenGLBufferPool) -> Unmanaged&lt;CFDictionary>?

Returns the attributes of OpenGL buffers that will be created from a buffer pool.

Deprecated


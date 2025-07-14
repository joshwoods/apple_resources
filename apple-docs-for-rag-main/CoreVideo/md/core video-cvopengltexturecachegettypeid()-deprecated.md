

- Core Video
-  CVOpenGLTextureCacheGetTypeID() Deprecated

Function

# CVOpenGLTextureCacheGetTypeID()

Returns the Core Foundation type identifier for a the texture cache.

macOS 10.4–10.14Deprecated

``` source
func CVOpenGLTextureCacheGetTypeID() -> CFTypeID
```

Deprecated

OpenGL/OpenGLES is no longer supported. Use Metal APIs instead. (Define COREVIDEO_SILENCE_GL_DEPRECATION to silence these warnings)

## See Also

### Functions

func CVOpenGLTextureCacheCreate(CFAllocator?, CFDictionary?, CGLContextObj, CGLPixelFormatObj, CFDictionary?, UnsafeMutablePointer&lt;CVOpenGLTextureCache?>) -> CVReturn

Creates a new texture cache.

Deprecated

func CVOpenGLTextureCacheCreateTextureFromImage(CFAllocator?, CVOpenGLTextureCache, CVImageBuffer, CFDictionary?, UnsafeMutablePointer&lt;CVOpenGLTexture?>) -> CVReturn

Creates a CVOpenGLTexture object from an existing CVImageBuffer.

Deprecated

func CVOpenGLTextureCacheFlush(CVOpenGLTextureCache, CVOptionFlags)

Performs internal housekeeping/recycling operations on the cache.

Deprecated


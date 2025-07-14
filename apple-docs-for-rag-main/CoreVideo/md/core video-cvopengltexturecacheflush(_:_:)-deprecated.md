

- Core Video
-  CVOpenGLTextureCacheFlush(\_:\_:) Deprecated

Function

# CVOpenGLTextureCacheFlush(\_:\_:)

Performs internal housekeeping/recycling operations on the cache.

macOS 10.4–10.14Deprecated

``` source
func CVOpenGLTextureCacheFlush(
    _ textureCache: CVOpenGLTextureCache,
    _ options: CVOptionFlags
)
```

Deprecated

OpenGL/OpenGLES is no longer supported. Use Metal APIs instead. (Define COREVIDEO_SILENCE_GL_DEPRECATION to silence these warnings)

## Parameters 

`textureCache`  

The texture cache object to flush.

`options`  

Currently unused, set to 0.

## Discussion

This call must be made periodically to give the texture cache a chance to make OpenGL calls on the OpenGL context used to create it in order to perform its required housekeeping operations.

## See Also

### Functions

func CVOpenGLTextureCacheCreate(CFAllocator?, CFDictionary?, CGLContextObj, CGLPixelFormatObj, CFDictionary?, UnsafeMutablePointer&lt;CVOpenGLTextureCache?>) -> CVReturn

Creates a new texture cache.

Deprecated

func CVOpenGLTextureCacheCreateTextureFromImage(CFAllocator?, CVOpenGLTextureCache, CVImageBuffer, CFDictionary?, UnsafeMutablePointer&lt;CVOpenGLTexture?>) -> CVReturn

Creates a CVOpenGLTexture object from an existing CVImageBuffer.

Deprecated

func CVOpenGLTextureCacheGetTypeID() -> CFTypeID

Returns the Core Foundation type identifier for a the texture cache.

Deprecated




- Core Video
-  CVOpenGLESTextureCacheFlush(\_:\_:) Deprecated

Function

# CVOpenGLESTextureCacheFlush(\_:\_:)

Performs internal housekeeping/recycling operations on a texture cache.

iOS 5.0–12.0DeprecatediPadOS 5.0–12.0DeprecatedtvOS 9.0–12.0Deprecated

``` source
func CVOpenGLESTextureCacheFlush(
    _ textureCache: CVOpenGLESTextureCache,
    _ options: CVOptionFlags
)
```

Deprecated

OpenGL/OpenGLES is no longer supported. Use Metal APIs instead. (Define COREVIDEO_SILENCE_GL_DEPRECATION to silence these warnings)

## Parameters 

`textureCache`  

The texture cache object to flush.

`options`  

Options for the flush operation. This parameter is currently unused and should be set to `0`.

## Discussion

The texture cache automatically flushes currently unused resources when you call the CVOpenGLESTextureCacheCreateTextureFromImage(_:_:_:_:_:_:_:_:_:_:_:_:) function, but can you can also flush the cache explicitly by calling this function. The EAGLContext associated with the cache may be used to delete or unbind textures.

## See Also

### Functions

func CVOpenGLESTextureCacheCreate(CFAllocator?, CFDictionary?, CVEAGLContext, CFDictionary?, UnsafeMutablePointer&lt;CVOpenGLESTextureCache?>) -> CVReturn

Creates a new Core Video texture cache.

Deprecated

func CVOpenGLESTextureCacheCreateTextureFromImage(CFAllocator?, CVOpenGLESTextureCache, CVImageBuffer, CFDictionary?, GLenum, GLint, GLsizei, GLsizei, GLenum, GLenum, Int, UnsafeMutablePointer&lt;CVOpenGLESTexture?>) -> CVReturn

Creates a CVOpenGLESTexture object from an existing CVImageBuffer.

Deprecated

func CVOpenGLESTextureCacheGetTypeID() -> CFTypeID

Returns the Core Foundation type identifier for a Core Video texture cache.

Deprecated


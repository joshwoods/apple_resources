

- Core Video
-  CVOpenGLESTextureCacheGetTypeID() Deprecated

Function

# CVOpenGLESTextureCacheGetTypeID()

Returns the Core Foundation type identifier for a Core Video texture cache.

iOS 5.0–12.0DeprecatediPadOS 5.0–12.0DeprecatedtvOS 9.0–12.0Deprecated

``` source
func CVOpenGLESTextureCacheGetTypeID() -> CFTypeID
```

Deprecated

OpenGL/OpenGLES is no longer supported. Use Metal APIs instead. (Define COREVIDEO_SILENCE_GL_DEPRECATION to silence these warnings)

## Return Value

The Core Foundation type identifier for the `CVOpenGLESTextureCacheRef` type.

## See Also

### Functions

func CVOpenGLESTextureCacheCreate(CFAllocator?, CFDictionary?, CVEAGLContext, CFDictionary?, UnsafeMutablePointer&lt;CVOpenGLESTextureCache?>) -> CVReturn

Creates a new Core Video texture cache.

Deprecated

func CVOpenGLESTextureCacheCreateTextureFromImage(CFAllocator?, CVOpenGLESTextureCache, CVImageBuffer, CFDictionary?, GLenum, GLint, GLsizei, GLsizei, GLenum, GLenum, Int, UnsafeMutablePointer&lt;CVOpenGLESTexture?>) -> CVReturn

Creates a CVOpenGLESTexture object from an existing CVImageBuffer.

Deprecated

func CVOpenGLESTextureCacheFlush(CVOpenGLESTextureCache, CVOptionFlags)

Performs internal housekeeping/recycling operations on a texture cache.

Deprecated


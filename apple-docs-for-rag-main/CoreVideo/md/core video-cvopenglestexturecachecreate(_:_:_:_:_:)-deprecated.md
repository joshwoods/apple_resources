

- Core Video
-  CVOpenGLESTextureCacheCreate(\_:\_:\_:\_:\_:) Deprecated

Function

# CVOpenGLESTextureCacheCreate(\_:\_:\_:\_:\_:)

Creates a new Core Video texture cache.

iOS 5.0–12.0DeprecatediPadOS 5.0–12.0DeprecatedtvOS 9.0–12.0Deprecated

``` source
func CVOpenGLESTextureCacheCreate(
    _ allocator: CFAllocator?,
    _ cacheAttributes: CFDictionary?,
    _ eaglContext: CVEAGLContext,
    _ textureAttributes: CFDictionary?,
    _ cacheOut: UnsafeMutablePointer
) -> CVReturn
```

Deprecated

OpenGL/OpenGLES is no longer supported. Use Metal APIs instead. (Define COREVIDEO_SILENCE_GL_DEPRECATION to silence these warnings)

## Parameters 

`allocator`  

The CFAllocator to use for allocating the texture cache. This parameter can be `NULL`.

`cacheAttributes`  

A CFDictionary containing the attributes of the texture cache itself. This parameter can be `NULL`.

`eaglContext`  

The OpenGLES 2.0 context into which the texture objects will be created. OpenGLES 1.x contexts are not supported.

`textureAttributes`  

A CFDictionary containing the attributes to be used for creating the CVOpenGLESTexture objects. This parameter can be `NULL`.

`cacheOut`  

A pointer to a `CVOpenGLESTextureCacheRef` where the newly created texture cache will be placed.

## Return Value

Upon successful creation of the texture cache, this function returns kCVReturnSuccess.

## See Also

### Functions

func CVOpenGLESTextureCacheCreateTextureFromImage(CFAllocator?, CVOpenGLESTextureCache, CVImageBuffer, CFDictionary?, GLenum, GLint, GLsizei, GLsizei, GLenum, GLenum, Int, UnsafeMutablePointer&lt;CVOpenGLESTexture?>) -> CVReturn

Creates a CVOpenGLESTexture object from an existing CVImageBuffer.

Deprecated

func CVOpenGLESTextureCacheFlush(CVOpenGLESTextureCache, CVOptionFlags)

Performs internal housekeeping/recycling operations on a texture cache.

Deprecated

func CVOpenGLESTextureCacheGetTypeID() -> CFTypeID

Returns the Core Foundation type identifier for a Core Video texture cache.

Deprecated


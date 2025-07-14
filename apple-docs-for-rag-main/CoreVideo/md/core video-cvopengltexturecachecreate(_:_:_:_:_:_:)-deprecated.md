

- Core Video
-  CVOpenGLTextureCacheCreate(\_:\_:\_:\_:\_:\_:) Deprecated

Function

# CVOpenGLTextureCacheCreate(\_:\_:\_:\_:\_:\_:)

Creates a new texture cache.

macOS 10.4–10.14Deprecated

``` source
func CVOpenGLTextureCacheCreate(
    _ allocator: CFAllocator?,
    _ cacheAttributes: CFDictionary?,
    _ cglContext: CGLContextObj,
    _ cglPixelFormat: CGLPixelFormatObj,
    _ textureAttributes: CFDictionary?,
    _ cacheOut: UnsafeMutablePointer
) -> CVReturn
```

Deprecated

OpenGL/OpenGLES is no longer supported. Use Metal APIs instead. (Define COREVIDEO_SILENCE_GL_DEPRECATION to silence these warnings)

## Parameters 

`allocator`  

The `CFAllocatorRef` to use for allocating the cache. May be NULL.

`cacheAttributes`  

A dictionary specifying options for the cache’s behavior, or `NULL` to use default options. For applicable keys and values, see Cache Attributes.

`cglContext`  

The OpenGL context into which the texture objects will be created.

`cglPixelFormat`  

The OpenGL pixel format object used to create the passed in OpenGL context.

`textureAttributes`  

A `CFDictionaryRef` containing the attributes to be used for creating the `CVOpenGLTexture` objects. May be `NULL`.

`cacheOut`  

Upon return, contains the newly created texture cache.

## Return Value

Returns kCVReturnSuccess on success.

## See Also

### Functions

func CVOpenGLTextureCacheCreateTextureFromImage(CFAllocator?, CVOpenGLTextureCache, CVImageBuffer, CFDictionary?, UnsafeMutablePointer&lt;CVOpenGLTexture?>) -> CVReturn

Creates a CVOpenGLTexture object from an existing CVImageBuffer.

Deprecated

func CVOpenGLTextureCacheFlush(CVOpenGLTextureCache, CVOptionFlags)

Performs internal housekeeping/recycling operations on the cache.

Deprecated

func CVOpenGLTextureCacheGetTypeID() -> CFTypeID

Returns the Core Foundation type identifier for a the texture cache.

Deprecated




- Core Video
-  CVOpenGLTextureCacheCreateTextureFromImage(\_:\_:\_:\_:\_:) Deprecated

Function

# CVOpenGLTextureCacheCreateTextureFromImage(\_:\_:\_:\_:\_:)

Creates a CVOpenGLTexture object from an existing CVImageBuffer.

macOS 10.4–10.14Deprecated

``` source
func CVOpenGLTextureCacheCreateTextureFromImage(
    _ allocator: CFAllocator?,
    _ textureCache: CVOpenGLTextureCache,
    _ sourceImage: CVImageBuffer,
    _ attributes: CFDictionary?,
    _ textureOut: UnsafeMutablePointer
) -> CVReturn
```

Deprecated

OpenGL/OpenGLES is no longer supported. Use Metal APIs instead. (Define COREVIDEO_SILENCE_GL_DEPRECATION to silence these warnings)

## Parameters 

`allocator`  

The `CFAllocatorRef` to use for allocating the `CVOpenGLTexture` object. May be `NULL`.

`textureCache`  

The texture cache object that will manage the texture.

`sourceImage`  

The source `CVImageBuffer` for which to create an `CVOpenGLTexture`.

`attributes`  

*This parameter is not currently supported and is for future use only.*

The desired buffer attributes for the `CVOpenGLTexture`.

`textureOut`  

Upon return, contains the newly created texture.

## Return Value

Returns kCVReturnSuccess on success.

## See Also

### Functions

func CVOpenGLTextureCacheCreate(CFAllocator?, CFDictionary?, CGLContextObj, CGLPixelFormatObj, CFDictionary?, UnsafeMutablePointer&lt;CVOpenGLTextureCache?>) -> CVReturn

Creates a new texture cache.

Deprecated

func CVOpenGLTextureCacheFlush(CVOpenGLTextureCache, CVOptionFlags)

Performs internal housekeeping/recycling operations on the cache.

Deprecated

func CVOpenGLTextureCacheGetTypeID() -> CFTypeID

Returns the Core Foundation type identifier for a the texture cache.

Deprecated


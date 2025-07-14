

- Core Video
-  CVMetalTextureCacheCreate(\_:\_:\_:\_:\_:) 

Function

# CVMetalTextureCacheCreate(\_:\_:\_:\_:\_:)

Creates a new texture cache.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
func CVMetalTextureCacheCreate(
    _ allocator: CFAllocator?,
    _ cacheAttributes: CFDictionary?,
    _ metalDevice: any MTLDevice,
    _ textureAttributes: CFDictionary?,
    _ cacheOut: UnsafeMutablePointer
) -> CVReturn
```

## Parameters 

`allocator`  

The memory allocator for the texture.

`cacheAttributes`  

A dictionary specifying options for the cache’s behavior, or `NULL` to use default options. For applicable keys and values, see Cache Attributes.

`metalDevice`  

The Metal device used to create texture objects.

`textureAttributes`  

A dictionary specifying options for creating textures from the cache, or `NULL` to use default options.

`cacheOut`  

Upon return, contains the newly created texture cache. When this value is `NULL`, an error occurred in texture creation.

## Return Value

Upon successful creation of the texture cache, this function returns kCVReturnSuccess.

## See Also

### Functions

func CVMetalTextureCacheCreateTextureFromImage(CFAllocator?, CVMetalTextureCache, CVImageBuffer, CFDictionary?, MTLPixelFormat, Int, Int, Int, UnsafeMutablePointer&lt;CVMetalTexture?>) -> CVReturn

Creates a Core Video Metal texture buffer from an existing image buffer.

func CVMetalTextureCacheFlush(CVMetalTextureCache, CVOptionFlags)

Manually flushes the contents of the provided texture cache.

func CVMetalTextureCacheGetTypeID() -> CFTypeID

Returns the Core Foundation type identifier for a Core Video Metal texture cache.


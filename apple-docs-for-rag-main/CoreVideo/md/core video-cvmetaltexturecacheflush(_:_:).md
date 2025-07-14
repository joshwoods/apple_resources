

- Core Video
-  CVMetalTextureCacheFlush(\_:\_:) 

Function

# CVMetalTextureCacheFlush(\_:\_:)

Manually flushes the contents of the provided texture cache.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
func CVMetalTextureCacheFlush(
    _ textureCache: CVMetalTextureCache,
    _ options: CVOptionFlags
)
```

## Parameters 

`textureCache`  

The texture cache object to flush.

`options`  

Options for the flush operation. This parameter is currently unused and should be `0`.

## Discussion

Texture caches automatically flush unused resources when you call the CVMetalTextureCacheCreateTextureFromImage(_:_:_:_:_:_:_:_:_:) function and on the time interval specified by kCVMetalTextureCacheMaximumTextureAgeKey. Use this method when you need fine-grained control over cache contents and memory.

## See Also

### Functions

func CVMetalTextureCacheCreate(CFAllocator?, CFDictionary?, any MTLDevice, CFDictionary?, UnsafeMutablePointer&lt;CVMetalTextureCache?>) -> CVReturn

Creates a new texture cache.

func CVMetalTextureCacheCreateTextureFromImage(CFAllocator?, CVMetalTextureCache, CVImageBuffer, CFDictionary?, MTLPixelFormat, Int, Int, Int, UnsafeMutablePointer&lt;CVMetalTexture?>) -> CVReturn

Creates a Core Video Metal texture buffer from an existing image buffer.

func CVMetalTextureCacheGetTypeID() -> CFTypeID

Returns the Core Foundation type identifier for a Core Video Metal texture cache.


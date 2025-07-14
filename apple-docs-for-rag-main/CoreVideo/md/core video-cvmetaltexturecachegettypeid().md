

- Core Video
-  CVMetalTextureCacheGetTypeID() 

Function

# CVMetalTextureCacheGetTypeID()

Returns the Core Foundation type identifier for a Core Video Metal texture cache.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
func CVMetalTextureCacheGetTypeID() -> CFTypeID
```

## Return Value

The Core Foundation type identifier for the `CVMetalTextureCacheRef` type.

## See Also

### Functions

func CVMetalTextureCacheCreate(CFAllocator?, CFDictionary?, any MTLDevice, CFDictionary?, UnsafeMutablePointer&lt;CVMetalTextureCache?>) -> CVReturn

Creates a new texture cache.

func CVMetalTextureCacheCreateTextureFromImage(CFAllocator?, CVMetalTextureCache, CVImageBuffer, CFDictionary?, MTLPixelFormat, Int, Int, Int, UnsafeMutablePointer&lt;CVMetalTexture?>) -> CVReturn

Creates a Core Video Metal texture buffer from an existing image buffer.

func CVMetalTextureCacheFlush(CVMetalTextureCache, CVOptionFlags)

Manually flushes the contents of the provided texture cache.


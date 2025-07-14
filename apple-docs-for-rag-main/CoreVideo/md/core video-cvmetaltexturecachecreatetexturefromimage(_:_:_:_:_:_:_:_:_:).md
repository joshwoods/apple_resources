

- Core Video
-  CVMetalTextureCacheCreateTextureFromImage(\_:\_:\_:\_:\_:\_:\_:\_:\_:) 

Function

# CVMetalTextureCacheCreateTextureFromImage(\_:\_:\_:\_:\_:\_:\_:\_:\_:)

Creates a Core Video Metal texture buffer from an existing image buffer.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
func CVMetalTextureCacheCreateTextureFromImage(
    _ allocator: CFAllocator?,
    _ textureCache: CVMetalTextureCache,
    _ sourceImage: CVImageBuffer,
    _ textureAttributes: CFDictionary?,
    _ pixelFormat: MTLPixelFormat,
    _ width: Int,
    _ height: Int,
    _ planeIndex: Int,
    _ textureOut: UnsafeMutablePointer
) -> CVReturn
```

## Parameters 

`allocator`  

The memory allocator for the texture.

`textureCache`  

The texture cache used to create and manage the texture.

`sourceImage`  

The Core Video image buffer from which to create a Metal texture.

`textureAttributes`  

A dictionary specifying options for creating the texture from the cache, or `NULL` to use default options.

`pixelFormat`  

The Metal pixel format constant describing the image buffer’s data.

`width`  

The width, in pixels, of the texture image.

`height`  

The height, in pixels, of the texture image.

`planeIndex`  

If the image buffer is planar, the index of the plane from which to map texture data. Ignored for non-planar image buffers.

`textureOut`  

Upon return, contains the newly created Metal texture buffer. When this value is `NULL`, an error occurred in texture creation.

## Return Value

Upon successful creation of the texture, this function returns kCVReturnSuccess.

## Discussion

This function creates a cached Core Video Metal texture object mapped to an image buffer, and a live binding to the underlying MTLTexture object.

Important

You need to maintain a strong reference to `textureOut` until the GPU finishes execution of commands accessing the texture, because the system doesn’t automatically retain it. Developers typically release these references in a block passed to addCompletedHandler(_:).

Note that Core Video doesn’t explicitly declare any pixel format types as Metal compatible. Specify true for the kCVPixelBufferMetalCompatibilityKey option to create Metal-compatible buffers when creating or requesting Core Video pixel buffers. You’re responsible for ensuring the pixel format is appropriate to the buffer.

The following code snippet demonstrates some example mappings:

```
```

## See Also

### Functions

func CVMetalTextureCacheCreate(CFAllocator?, CFDictionary?, any MTLDevice, CFDictionary?, UnsafeMutablePointer&lt;CVMetalTextureCache?>) -> CVReturn

Creates a new texture cache.

func CVMetalTextureCacheFlush(CVMetalTextureCache, CVOptionFlags)

Manually flushes the contents of the provided texture cache.

func CVMetalTextureCacheGetTypeID() -> CFTypeID

Returns the Core Foundation type identifier for a Core Video Metal texture cache.


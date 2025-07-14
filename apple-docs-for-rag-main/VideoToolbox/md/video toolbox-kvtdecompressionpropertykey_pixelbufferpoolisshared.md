

- Video Toolbox
-  kVTDecompressionPropertyKey_PixelBufferPoolIsShared 

Global Variable

# kVTDecompressionPropertyKey_PixelBufferPoolIsShared

A Boolean value indicating whether a common pixel buffer pool is shared between the video decoder and the session client.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.8+tvOS 10.2+visionOS 1.0+

``` source
let kVTDecompressionPropertyKey_PixelBufferPoolIsShared: CFString
```

## Discussion

This value is false if separate pools are used because the pixel buffer attributes specified by the video decoder and the client are incompatible.

## See Also

### Pixel Buffer Pools

let kVTDecompressionPropertyKey_PixelBufferPool: CFString

A pixel buffer pool for pixel buffers being output by the decompression session.

let kVTDecompressionPropertyKey_OutputPoolRequestedMinimumBufferCount: CFString

The requested minimum buffer count that a decompression session should use for its output pixel buffer pool, without releasing buffers while the number in use is below this level.


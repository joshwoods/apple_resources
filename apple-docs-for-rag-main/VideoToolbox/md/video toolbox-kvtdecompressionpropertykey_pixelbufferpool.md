

- Video Toolbox
-  kVTDecompressionPropertyKey_PixelBufferPool 

Global Variable

# kVTDecompressionPropertyKey_PixelBufferPool

A pixel buffer pool for pixel buffers being output by the decompression session.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.8+tvOS 10.2+visionOS 1.0+

``` source
let kVTDecompressionPropertyKey_PixelBufferPool: CFString
```

## Discussion

This pixel buffer pool is always compatible with the client’s pixel buffer attributes as specified when calling VTDecompressionSessionCreate(allocator:formatDescription:decoderSpecification:imageBufferAttributes:outputCallback:decompressionSessionOut:).

## See Also

### Pixel Buffer Pools

let kVTDecompressionPropertyKey_PixelBufferPoolIsShared: CFString

A Boolean value indicating whether a common pixel buffer pool is shared between the video decoder and the session client.

let kVTDecompressionPropertyKey_OutputPoolRequestedMinimumBufferCount: CFString

The requested minimum buffer count that a decompression session should use for its output pixel buffer pool, without releasing buffers while the number in use is below this level.




- Video Toolbox
-  kVTDecompressionPropertyKey_OutputPoolRequestedMinimumBufferCount 

Global Variable

# kVTDecompressionPropertyKey_OutputPoolRequestedMinimumBufferCount

The requested minimum buffer count that a decompression session should use for its output pixel buffer pool, without releasing buffers while the number in use is below this level.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.9+tvOS 10.2+visionOS 1.0+

``` source
let kVTDecompressionPropertyKey_OutputPoolRequestedMinimumBufferCount: CFString
```

## Discussion

This property effectively requests that the kCVPixelBufferPoolMinimumBufferCountKey key be used for the creation of the output CVPixelBufferPool.

For general playback cases, standard CVPixelBufferPool age-out behavior is sufficient, and this property isn’t necessary. Use this property only in unusual playback scenarios where a peak pool level is known, and the potential memory overhead is an acceptable tradeoff to avoid possible buffer reallocation. Setting this property to `NULL` or passing in the value `0` clears this setting and removes the minimum buffer count.

Setting this property while a decompression session is in use results in the creation of a new CVPixelBufferPool. Setting this property causes new buffers to be allocated, and existing buffers to be deallocated when they are released.

## See Also

### Pixel Buffer Pools

let kVTDecompressionPropertyKey_PixelBufferPool: CFString

A pixel buffer pool for pixel buffers being output by the decompression session.

let kVTDecompressionPropertyKey_PixelBufferPoolIsShared: CFString

A Boolean value indicating whether a common pixel buffer pool is shared between the video decoder and the session client.


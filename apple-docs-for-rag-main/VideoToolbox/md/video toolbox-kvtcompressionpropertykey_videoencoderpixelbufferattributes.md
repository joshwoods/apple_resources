

- Video Toolbox
-  kVTCompressionPropertyKey_VideoEncoderPixelBufferAttributes 

Global Variable

# kVTCompressionPropertyKey_VideoEncoderPixelBufferAttributes

The video encoder’s pixel buffer attributes for the compression session.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.8+tvOS 10.2+visionOS 1.0+

``` source
let kVTCompressionPropertyKey_VideoEncoderPixelBufferAttributes: CFString
```

## Discussion

You can use these attributes to create a pixel buffer pool for source pixel buffers.

## See Also

### Buffers

let kVTCompressionPropertyKey_NumberOfPendingFrames: CFString

The number of pending frames in the compression session.

let kVTCompressionPropertyKey_PixelBufferPoolIsShared: CFString

A Boolean value indicating whether the common pixel buffer pool is shared between the video encoder and the session client.


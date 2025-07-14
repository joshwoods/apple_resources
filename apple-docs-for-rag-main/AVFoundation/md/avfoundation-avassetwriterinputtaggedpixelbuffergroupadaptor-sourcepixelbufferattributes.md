

- AVFoundation
- AVAssetWriterInputTaggedPixelBufferGroupAdaptor
-  sourcePixelBufferAttributes 

Instance Property

# sourcePixelBufferAttributes

The attributes of buffers that the adaptor’s pixel buffer pool vends.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+visionOS 1.0+

``` source
var sourcePixelBufferAttributes: [String : Any]? { get }
```

## Discussion

The value of this property is a dictionary containing pixel buffer attribute keys defined in ``.

## See Also

### Configuring the buffer pool

var pixelBufferPool: CVPixelBufferPool?

A pixel buffer pool that vends and efficiently recycles the pixel buffers of tagged buffer groups.


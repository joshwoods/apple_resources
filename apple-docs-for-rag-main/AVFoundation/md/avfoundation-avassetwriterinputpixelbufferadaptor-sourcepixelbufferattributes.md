

- AVFoundation
- AVAssetWriterInputPixelBufferAdaptor
-  sourcePixelBufferAttributes 

Instance Property

# sourcePixelBufferAttributes

The attributes of the pixel buffers that the pool contains.

iOS 4.1+iPadOS 4.1+Mac Catalyst 13.1+macOS 10.7+tvOS 9.0+visionOS 1.0+

``` source
var sourcePixelBufferAttributes: [String : Any]? { get }
```

## See Also

### Accessing the Pool

var pixelBufferPool: CVPixelBufferPool?

A pool of pixel buffers to append to the adaptor’s input.


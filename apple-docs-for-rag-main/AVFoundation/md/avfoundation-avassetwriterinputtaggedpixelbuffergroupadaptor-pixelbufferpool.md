

- AVFoundation
- AVAssetWriterInputTaggedPixelBufferGroupAdaptor
-  pixelBufferPool 

Instance Property

# pixelBufferPool

A pixel buffer pool that vends and efficiently recycles the pixel buffers of tagged buffer groups.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+visionOS 1.0+

``` source
var pixelBufferPool: CVPixelBufferPool? { get }
```

## Discussion

For maximum efficiency, create the pixel buffers of tagged buffer groups using this pool with the CVPixelBufferPoolCreatePixelBuffer(_:_:_:) function.

The value of this property is `nil` before you call startWriting() on the associated AVAssetWriter object. Query this property after writing starts to retrieve a `non-nil` value.

This property is not key value observable.

## See Also

### Configuring the buffer pool

var sourcePixelBufferAttributes: [String : Any]?

The attributes of buffers that the adaptor’s pixel buffer pool vends.


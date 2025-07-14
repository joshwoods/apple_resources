

- AVFoundation
- AVAssetWriterInputPixelBufferAdaptor
-  pixelBufferPool 

Instance Property

# pixelBufferPool

A pool of pixel buffers to append to the adaptor’s input.

iOS 4.1+iPadOS 4.1+Mac Catalyst 13.1+macOS 10.7+tvOS 9.0+visionOS 1.0+

``` source
var pixelBufferPool: CVPixelBufferPool? { get }
```

## Discussion

For maximum efficiency, you should create CVPixelBuffer objects for append(_:withPresentationTime:) by using this pool with the CVPixelBufferPoolCreatePixelBuffer(_:_:_:) function.

This value is `nil` prior to calling startSession(atSourceTime:)on the associated AVAssetWriter object.

This property is key-value observable.

## See Also

### Accessing the Pool

var sourcePixelBufferAttributes: [String : Any]?

The attributes of the pixel buffers that the pool contains.


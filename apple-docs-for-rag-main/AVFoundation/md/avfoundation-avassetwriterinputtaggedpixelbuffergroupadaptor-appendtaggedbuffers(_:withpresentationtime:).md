

- AVFoundation
- AVAssetWriterInputTaggedPixelBufferGroupAdaptor
-  appendTaggedBuffers(\_:withPresentationTime:) 

Instance Method

# appendTaggedBuffers(\_:withPresentationTime:)

Appends a tagged buffer group to the adaptor.

iOS 17.0+iPadOS 17.0+Mac CatalystmacOS 14.0+visionOS 1.0+

``` source
func appendTaggedBuffers(
    _ taggedBuffers: [CMTaggedBuffer],
    withPresentationTime: CMTime
) -> Bool
```

## See Also

### Appending pixel buffers

func appendTaggedPixelBufferGroup(__CMTaggedBufferGroup, withPresentationTime: CMTime) -> Bool

Appends a tagged buffer group to the adaptor.


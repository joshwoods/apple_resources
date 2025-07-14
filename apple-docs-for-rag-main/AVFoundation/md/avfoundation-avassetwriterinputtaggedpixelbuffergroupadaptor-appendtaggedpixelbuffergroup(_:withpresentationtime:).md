

- AVFoundation
- AVAssetWriterInputTaggedPixelBufferGroupAdaptor
-  appendTaggedPixelBufferGroup(\_:withPresentationTime:) 

Instance Method

# appendTaggedPixelBufferGroup(\_:withPresentationTime:)

Appends a tagged buffer group to the adaptor.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+visionOS 1.0+

``` source
func appendTaggedPixelBufferGroup(
    _ taggedPixelBufferGroup: __CMTaggedBufferGroup,
    withPresentationTime presentationTime: CMTime
) -> Bool
```

## See Also

### Appending pixel buffers

func appendTaggedBuffers([CMTaggedBuffer], withPresentationTime: CMTime) -> Bool

Appends a tagged buffer group to the adaptor.


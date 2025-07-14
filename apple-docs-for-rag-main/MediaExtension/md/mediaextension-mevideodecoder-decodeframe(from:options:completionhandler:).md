

- MediaExtension
- MEVideoDecoder
-  decodeFrame(from:options:completionHandler:) 

Instance Method

# decodeFrame(from:options:completionHandler:)

Requests the extension to decode a video frame.

macOS 14.0+

``` source
func decodeFrame(
    from sampleBuffer: CMSampleBuffer,
    options: MEDecodeFrameOptions,
    completionHandler: @escaping (CVImageBuffer?, MEDecodeFrameStatus, (any Error)?) -> Void
)
```

``` source
func decodeFrame(
    from sampleBuffer: CMSampleBuffer,
    options: MEDecodeFrameOptions
) async throws -> (CVImageBuffer, MEDecodeFrameStatus)
```

**Required**

## Parameters 

`sampleBuffer`  

A sample buffer that contains one video frame.

`options`  

Specific decode options for the frame.

`completionHandler`  

The completion block to execute when the decode operation finishes.

## Discussion

This method calls the completion handler for every sample buffer frame when decoding completes, but not necessarily in display order. The completion handler receives a decoded pixel buffer, a decode status that indicates a frame dropped, or an error. Use MEVideoDecoderPixelBufferManager to allocate an image buffer. If an error occurs that’s external to MediaExtensionErrorDomain, the VTDecompressionSession receives it as kVTVideoDecoderUnknownErr.

## See Also

### Decoding frames

func canAccept(CMFormatDescription) -> Bool

Asks the extension whether the decoder can decode frames with the format description that you specify.

struct MEDecodeFrameStatus

A type that represents a non-error status related to a frame decode operation.


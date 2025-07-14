

- MediaExtension
- MEVideoDecoder
-  canAccept(\_:) 

Instance Method

# canAccept(\_:)

Asks the extension whether the decoder can decode frames with the format description that you specify.

macOS 14.0+

``` source
optional func canAccept(_ formatDescription: CMFormatDescription) -> Bool
```

## Parameters 

`formatDescription`  

The new format description to evaluate.

## See Also

### Decoding frames

func decodeFrame(from: CMSampleBuffer, options: MEDecodeFrameOptions, completionHandler: (CVImageBuffer?, MEDecodeFrameStatus, (any Error)?) -> Void)

Requests the extension to decode a video frame.

**Required**

struct MEDecodeFrameStatus

A type that represents a non-error status related to a frame decode operation.


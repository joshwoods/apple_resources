

- AVFoundation
- AVCaptureDevice
- AVCaptureDevice.Format
-  isVideoHDRSupported 

Instance Property

# isVideoHDRSupported

A Boolean value that indicates whether the format supports high dynamic range streaming.

iOS 8.0+iPadOS 8.0+Mac Catalyst 14.0+tvOS 17.0+

``` source
var isVideoHDRSupported: Bool { get }
```

## See Also

### Determining Video Capture Support

var isAutoVideoFrameRateSupported: Bool

A Boolean value that Indicates whether the format supports performing automatic video frame rate adjustments.

var videoSupportedFrameRateRanges: [AVFrameRateRange]

A list of frame rate ranges that a format supports.

class AVFrameRateRange

An immutable type that represents a range of valid frame rates.

var isVideoBinned: Bool

A Boolean value that indicates whether the format produces video data in a binned format.

var isMultiCamSupported: Bool

A Boolean value that indicates whether a multi-camera capture session supports this format.




- AVFoundation
- AVCaptureDevice
- AVCaptureDevice.Format
-  videoSupportedFrameRateRanges 

Instance Property

# videoSupportedFrameRateRanges

A list of frame rate ranges that a format supports.

iOS 7.0+iPadOS 7.0+Mac Catalyst 14.0+macOS 10.7+tvOS 17.0+visionOS 1.0+

``` source
var videoSupportedFrameRateRanges: [AVFrameRateRange] { get }
```

## Discussion

The value is an array of AVFrameRateRange objects, one for each of the format’s supported video frame rate ranges.

## See Also

### Determining Video Capture Support

var isAutoVideoFrameRateSupported: Bool

A Boolean value that Indicates whether the format supports performing automatic video frame rate adjustments.

class AVFrameRateRange

An immutable type that represents a range of valid frame rates.

var isVideoBinned: Bool

A Boolean value that indicates whether the format produces video data in a binned format.

var isVideoHDRSupported: Bool

A Boolean value that indicates whether the format supports high dynamic range streaming.

var isMultiCamSupported: Bool

A Boolean value that indicates whether a multi-camera capture session supports this format.


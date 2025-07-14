

- AVFoundation
- AVCaptureDevice
- AVCaptureDevice.Format
-  isVideoBinned 

Instance Property

# isVideoBinned

A Boolean value that indicates whether the format produces video data in a binned format.

iOS 7.0+iPadOS 7.0+Mac Catalyst 14.0+tvOS 17.0+

``` source
var isVideoBinned: Bool { get }
```

## Discussion

Binning is a pixel-combining process which can result in greater low light sensitivity at the cost of reduced resolution.

## See Also

### Determining Video Capture Support

var isAutoVideoFrameRateSupported: Bool

A Boolean value that Indicates whether the format supports performing automatic video frame rate adjustments.

var videoSupportedFrameRateRanges: [AVFrameRateRange]

A list of frame rate ranges that a format supports.

class AVFrameRateRange

An immutable type that represents a range of valid frame rates.

var isVideoHDRSupported: Bool

A Boolean value that indicates whether the format supports high dynamic range streaming.

var isMultiCamSupported: Bool

A Boolean value that indicates whether a multi-camera capture session supports this format.


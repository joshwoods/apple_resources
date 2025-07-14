

- AVFoundation
- AVCaptureDevice
- AVCaptureDevice.Format
-  isAutoVideoFrameRateSupported 

Instance Property

# isAutoVideoFrameRateSupported

A Boolean value that Indicates whether the format supports performing automatic video frame rate adjustments.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+

``` source
var isAutoVideoFrameRateSupported: Bool { get }
```

## Discussion

This property determines whether you can enable a capture device’s isAutoVideoFrameRateEnabled property.

## See Also

### Determining Video Capture Support

var videoSupportedFrameRateRanges: [AVFrameRateRange]

A list of frame rate ranges that a format supports.

class AVFrameRateRange

An immutable type that represents a range of valid frame rates.

var isVideoBinned: Bool

A Boolean value that indicates whether the format produces video data in a binned format.

var isVideoHDRSupported: Bool

A Boolean value that indicates whether the format supports high dynamic range streaming.

var isMultiCamSupported: Bool

A Boolean value that indicates whether a multi-camera capture session supports this format.


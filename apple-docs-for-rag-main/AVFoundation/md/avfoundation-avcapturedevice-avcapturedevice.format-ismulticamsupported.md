

- AVFoundation
- AVCaptureDevice
- AVCaptureDevice.Format
-  isMultiCamSupported 

Instance Property

# isMultiCamSupported

A Boolean value that indicates whether a multi-camera capture session supports this format.

iOS 13.0+iPadOS 13.0+Mac Catalyst 14.0+tvOS 17.0+

``` source
var isMultiCamSupported: Bool { get }
```

## Discussion

When performing single-camera capture using AVCaptureSession, you may set any of the device’s formats as its activeFormat. However, when using AVCaptureMultiCamSession, you may only set the device’s format to one in which isMultiCamSupported is true. Only this limited subset of capture formats can run sustainably in a multi-camera capture scenario.

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

var isVideoHDRSupported: Bool

A Boolean value that indicates whether the format supports high dynamic range streaming.


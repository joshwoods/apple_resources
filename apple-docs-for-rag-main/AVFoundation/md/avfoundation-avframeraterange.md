

- AVFoundation
-  AVFrameRateRange 

Class

# AVFrameRateRange

An immutable type that represents a range of valid frame rates.

iOS 7.0+iPadOS 7.0+Mac Catalyst 14.0+macOS 10.7+tvOS 17.0+visionOS 1.0+

``` source
class AVFrameRateRange
```

## Overview

An AVFrameRateRange object is immutable.

An AVCaptureDevice.Format object wraps a CMFormatDescription and expresses a range of valid video frame rates as an array of `AVFrameRateRange` objects.

An AVCaptureDevice object uses `AVCaptureDeviceFormat` to describe the formats it supports and the currently-active format.

## Topics

### Accessing Properties

var maxFrameDuration: CMTime

The maximum frame duration supported by the range.

var maxFrameRate: Float64

The maximum frame rate supported by the range.

var minFrameDuration: CMTime

The minimum frame duration supported by the range.

var minFrameRate: Float64

The minimum frame rate supported by the range.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

## See Also

### Determining Video Capture Support

var isAutoVideoFrameRateSupported: Bool

A Boolean value that Indicates whether the format supports performing automatic video frame rate adjustments.

var videoSupportedFrameRateRanges: [AVFrameRateRange]

A list of frame rate ranges that a format supports.

var isVideoBinned: Bool

A Boolean value that indicates whether the format produces video data in a binned format.

var isVideoHDRSupported: Bool

A Boolean value that indicates whether the format supports high dynamic range streaming.

var isMultiCamSupported: Bool

A Boolean value that indicates whether a multi-camera capture session supports this format.


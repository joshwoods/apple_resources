

- ARKit
- ARConfiguration
-  ARConfiguration.VideoFormat 

Class

# ARConfiguration.VideoFormat

A video size and frame rate specification for use with an AR session.

iOS 11.3+iPadOS 11.3+Mac Catalyst 13.1+

``` source
class VideoFormat
```

## Overview

This class is immutable; to set the frame rate and video resolution for an AR session, set your configuration’s videoFormat property to one of the formats in the supportedVideoFormats array.

## Topics

### Accessing format information

var framesPerSecond: Int

The rate at which the session captures video and provides AR frame information.

var imageResolution: CGSize

The size, in pixels, of video images captured in the session.

var isRecommendedForHighResolutionFrameCapturing: Bool

Determines whether the framework considers a format suitable for high-resolution frame capture.

var isVideoHDRSupported: Bool

Determines whether the format supports high dynamic range (HDR).

### Inspecting the video source

var captureDevicePosition: AVCaptureDevice.Position

The position of the capture device.

enum AVCaptureDevice.Position

Constants that indicate the physical position of a capture device.

var captureDeviceType: AVCaptureDevice.DeviceType

The camera that supplies the video format.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCopying
- NSObjectProtocol

## See Also

### Managing video capture options

var videoFormat: ARConfiguration.VideoFormat

Video format of the session output.

class var supportedVideoFormats: [ARConfiguration.VideoFormat]

The set of video capture formats available on the current device.

var videoHDRAllowed: Bool

Enables high dynamic range (HDR) for the session’s camera feed.

class var configurableCaptureDeviceForPrimaryCamera: AVCaptureDevice?

An object that enables you to alter the appearance of a frame’s captured image.

class var recommendedVideoFormatFor4KResolution: ARConfiguration.VideoFormat?

Provides a 4K video format if the device and configuration support it.

class var recommendedVideoFormatForHighResolutionFrameCapturing: ARConfiguration.VideoFormat?

Returns a video format that the framework recommends for high-resolution-still-image capture.


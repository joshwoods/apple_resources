

- ARKit
- ARConfiguration
-  videoHDRAllowed 

Instance Property

# videoHDRAllowed

Enables high dynamic range (HDR) for the session’s camera feed.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+

``` source
var videoHDRAllowed: Bool { get set }
```

## Discussion

Before calling this function, check whether the session configuration’s video format supports HDR first by calling isVideoHDRSupported.

## See Also

### Managing video capture options

var videoFormat: ARConfiguration.VideoFormat

Video format of the session output.

class var supportedVideoFormats: [ARConfiguration.VideoFormat]

The set of video capture formats available on the current device.

class VideoFormat

A video size and frame rate specification for use with an AR session.

class var configurableCaptureDeviceForPrimaryCamera: AVCaptureDevice?

An object that enables you to alter the appearance of a frame’s captured image.

class var recommendedVideoFormatFor4KResolution: ARConfiguration.VideoFormat?

Provides a 4K video format if the device and configuration support it.

class var recommendedVideoFormatForHighResolutionFrameCapturing: ARConfiguration.VideoFormat?

Returns a video format that the framework recommends for high-resolution-still-image capture.


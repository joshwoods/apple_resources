

- ARKit
- ARConfiguration
-  videoFormat 

Instance Property

# videoFormat

Video format of the session output.

iOS 11.3+iPadOS 11.3+Mac Catalyst 13.1+

``` source
var videoFormat: ARConfiguration.VideoFormat { get set }
```

## See Also

### Managing video capture options

class var supportedVideoFormats: [ARConfiguration.VideoFormat]

The set of video capture formats available on the current device.

class VideoFormat

A video size and frame rate specification for use with an AR session.

var videoHDRAllowed: Bool

Enables high dynamic range (HDR) for the session’s camera feed.

class var configurableCaptureDeviceForPrimaryCamera: AVCaptureDevice?

An object that enables you to alter the appearance of a frame’s captured image.

class var recommendedVideoFormatFor4KResolution: ARConfiguration.VideoFormat?

Provides a 4K video format if the device and configuration support it.

class var recommendedVideoFormatForHighResolutionFrameCapturing: ARConfiguration.VideoFormat?

Returns a video format that the framework recommends for high-resolution-still-image capture.




- ARKit
- ARConfiguration
-  recommendedVideoFormatFor4KResolution 

Type Property

# recommendedVideoFormatFor4KResolution

Provides a 4K video format if the device and configuration support it.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+

``` source
class var recommendedVideoFormatFor4KResolution: ARConfiguration.VideoFormat? { get }
```

## Discussion

If the device and configuration support 4K, the returned video format is also present in the configuration’s supportedVideoFormats array.

This function returns `nil` if the device or configuration doesn’t support 4K, so you can call this function to determine whether to enable 4K for your session.

## See Also

### Managing video capture options

var videoFormat: ARConfiguration.VideoFormat

Video format of the session output.

class var supportedVideoFormats: [ARConfiguration.VideoFormat]

The set of video capture formats available on the current device.

class VideoFormat

A video size and frame rate specification for use with an AR session.

var videoHDRAllowed: Bool

Enables high dynamic range (HDR) for the session’s camera feed.

class var configurableCaptureDeviceForPrimaryCamera: AVCaptureDevice?

An object that enables you to alter the appearance of a frame’s captured image.

class var recommendedVideoFormatForHighResolutionFrameCapturing: ARConfiguration.VideoFormat?

Returns a video format that the framework recommends for high-resolution-still-image capture.


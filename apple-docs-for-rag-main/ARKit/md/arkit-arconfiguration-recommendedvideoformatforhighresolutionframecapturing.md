

- ARKit
- ARConfiguration
-  recommendedVideoFormatForHighResolutionFrameCapturing 

Type Property

# recommendedVideoFormatForHighResolutionFrameCapturing

Returns a video format that the framework recommends for high-resolution-still-image capture.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+

``` source
class var recommendedVideoFormatForHighResolutionFrameCapturing: ARConfiguration.VideoFormat? { get }
```

## Discussion

The framework determines the resolution of the camera feed and still-image capture for this format. Call this function when your app requires a high-resolution still capture regardless of format specifics. If instead, your app requires a particular resolution, iterate over the supportedVideoFormats array and choose a format with the desired configuration where isRecommendedForHighResolutionFrameCapturing is `true`.

Other video formats may support still-image capture but at a lower quality or resolution.

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

class var recommendedVideoFormatFor4KResolution: ARConfiguration.VideoFormat?

Provides a 4K video format if the device and configuration support it.


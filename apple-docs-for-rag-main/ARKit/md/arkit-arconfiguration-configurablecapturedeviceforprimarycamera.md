

- ARKit
- ARConfiguration
-  configurableCaptureDeviceForPrimaryCamera 

Type Property

# configurableCaptureDeviceForPrimaryCamera

An object that enables you to alter the appearance of a frame’s captured image.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+

``` source
class var configurableCaptureDeviceForPrimaryCamera: AVCaptureDevice? { get }
```

## Discussion

This property provides the underlying capture device for the framework’s camera feed. By altering the device’s configuration, your app indirectly adjusts the visual properties of the each AR frame’s capturedImage.

Alter the device’s settings with caution, as extreme changes can affect ARKit’s features that rely on the capturedImage and depend on its integrity, such as people occlusion that uses personSegmentation.

Important

This property is `nil` on devices that aren’t equiped with an ultra-wide camera.

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

class var recommendedVideoFormatFor4KResolution: ARConfiguration.VideoFormat?

Provides a 4K video format if the device and configuration support it.

class var recommendedVideoFormatForHighResolutionFrameCapturing: ARConfiguration.VideoFormat?

Returns a video format that the framework recommends for high-resolution-still-image capture.


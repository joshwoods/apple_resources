

- ARKit
- ARConfiguration
-  supportedVideoFormats 

Type Property

# supportedVideoFormats

The set of video capture formats available on the current device.

iOS 11.3+iPadOS 11.3+Mac Catalyst 13.1+

``` source
class var supportedVideoFormats: [ARConfiguration.VideoFormat] { get }
```

## Discussion

By default, the videoFormat property for a new session configuration matches the first video capture format in this array. To change the video format for a session, change that property’s value to one of the other ARConfiguration.VideoFormat objects in this array.

Important

ARConfiguration is an abstract base class, so its implementation of this property always returns an empty array. Read this property from the configuration subclass you plan to use for your AR session, such as ARWorldTrackingConfiguration or ARFaceTrackingConfiguration.

Different devices and iOS versions offer different sets of supported video formats, but the order of this array always puts higher-quality formats before lower-quality formats. For best results across all devices and versions, choose formats based on their order in the array rather than on hard-coded minimum resolution or frame rate values.

## See Also

### Managing video capture options

var videoFormat: ARConfiguration.VideoFormat

Video format of the session output.

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




- ARKit
- ARConfiguration
- ARConfiguration.VideoFormat
-  imageResolution 

Instance Property

# imageResolution

The size, in pixels, of video images captured in the session.

iOS 11.3+iPadOS 11.3+Mac Catalyst 13.1+

``` source
var imageResolution: CGSize { get }
```

## Discussion

Video format sizes are relative to the native sensor orientation of the device camera, and as such are always landscape-oriented.

## See Also

### Accessing format information

var framesPerSecond: Int

The rate at which the session captures video and provides AR frame information.

var isRecommendedForHighResolutionFrameCapturing: Bool

Determines whether the framework considers a format suitable for high-resolution frame capture.

var isVideoHDRSupported: Bool

Determines whether the format supports high dynamic range (HDR).


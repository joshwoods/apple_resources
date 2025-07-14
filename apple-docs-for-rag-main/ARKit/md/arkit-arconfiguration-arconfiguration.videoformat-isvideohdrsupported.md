

- ARKit
- ARConfiguration
- ARConfiguration.VideoFormat
-  isVideoHDRSupported 

Instance Property

# isVideoHDRSupported

Determines whether the format supports high dynamic range (HDR).

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+

``` source
var isVideoHDRSupported: Bool { get }
```

## Discussion

Call this function before setting videoHDRAllowed to `true` to first check whether a video format supports HDR.

## See Also

### Accessing format information

var framesPerSecond: Int

The rate at which the session captures video and provides AR frame information.

var imageResolution: CGSize

The size, in pixels, of video images captured in the session.

var isRecommendedForHighResolutionFrameCapturing: Bool

Determines whether the framework considers a format suitable for high-resolution frame capture.


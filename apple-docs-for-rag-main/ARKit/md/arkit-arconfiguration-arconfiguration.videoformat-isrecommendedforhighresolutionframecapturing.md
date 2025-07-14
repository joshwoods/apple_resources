

- ARKit
- ARConfiguration
- ARConfiguration.VideoFormat
-  isRecommendedForHighResolutionFrameCapturing 

Instance Property

# isRecommendedForHighResolutionFrameCapturing

Determines whether the framework considers a format suitable for high-resolution frame capture.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+

``` source
var isRecommendedForHighResolutionFrameCapturing: Bool { get }
```

## See Also

### Accessing format information

var framesPerSecond: Int

The rate at which the session captures video and provides AR frame information.

var imageResolution: CGSize

The size, in pixels, of video images captured in the session.

var isVideoHDRSupported: Bool

Determines whether the format supports high dynamic range (HDR).


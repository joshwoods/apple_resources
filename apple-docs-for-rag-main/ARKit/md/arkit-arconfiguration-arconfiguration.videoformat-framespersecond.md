

- ARKit
- ARConfiguration
- ARConfiguration.VideoFormat
-  framesPerSecond 

Instance Property

# framesPerSecond

The rate at which the session captures video and provides AR frame information.

iOS 11.3+iPadOS 11.3+Mac Catalyst 13.1+

``` source
var framesPerSecond: Int { get }
```

## See Also

### Accessing format information

var imageResolution: CGSize

The size, in pixels, of video images captured in the session.

var isRecommendedForHighResolutionFrameCapturing: Bool

Determines whether the framework considers a format suitable for high-resolution frame capture.

var isVideoHDRSupported: Bool

Determines whether the format supports high dynamic range (HDR).


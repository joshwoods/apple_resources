

- AVFoundation
- AVCaptureConnection
-  isVideoStabilizationEnabled Deprecated

Instance Property

# isVideoStabilizationEnabled

A Boolean value that indicates whether video stabilization is active for the connection.

iOS 6.0–8.0DeprecatediPadOS 6.0–8.0DeprecatedMac Catalyst 13.1–13.1Deprecated

``` source
var isVideoStabilizationEnabled: Bool { get }
```

Deprecated

Use the activeVideoStabilizationMode property instead.

## See Also

### Deprecated

var enablesVideoStabilizationWhenAvailable: Bool

A Boolean value that indicates whether the system enables video stabilization when it’s available.

Deprecated

var isVideoOrientationSupported: Bool

A Boolean value that indicates whether the connection supports changing the orientation of the video.

Deprecated

var videoOrientation: AVCaptureVideoOrientation

An orientation that tells the connection how to rotate a video flowing through it.

Deprecated

enum AVCaptureVideoOrientation

Constants indicating video orientation.

Deprecated


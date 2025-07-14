

- AVFoundation
- AVCaptureConnection
-  isVideoOrientationSupported Deprecated

Instance Property

# isVideoOrientationSupported

A Boolean value that indicates whether the connection supports changing the orientation of the video.

iOS 4.0–17.0DeprecatediPadOS 4.0–17.0DeprecatedMac Catalyst 14.0–17.0DeprecatedmacOS 10.7–14.0Deprecated

``` source
var isVideoOrientationSupported: Bool { get }
```

Deprecated

Use isVideoRotationAngleSupported(_:) instead.

## See Also

### Deprecated

var isVideoStabilizationEnabled: Bool

A Boolean value that indicates whether video stabilization is active for the connection.

Deprecated

var enablesVideoStabilizationWhenAvailable: Bool

A Boolean value that indicates whether the system enables video stabilization when it’s available.

Deprecated

var videoOrientation: AVCaptureVideoOrientation

An orientation that tells the connection how to rotate a video flowing through it.

Deprecated

enum AVCaptureVideoOrientation

Constants indicating video orientation.

Deprecated




- AVFoundation
- AVCaptureConnection
-  enablesVideoStabilizationWhenAvailable Deprecated

Instance Property

# enablesVideoStabilizationWhenAvailable

A Boolean value that indicates whether the system enables video stabilization when it’s available.

iOS 6.0–8.0DeprecatediPadOS 6.0–8.0DeprecatedMac Catalyst 13.1–13.1Deprecated

``` source
var enablesVideoStabilizationWhenAvailable: Bool { get set }
```

Deprecated

Use the preferredVideoStabilizationMode property instead.

## See Also

### Deprecated

var isVideoStabilizationEnabled: Bool

A Boolean value that indicates whether video stabilization is active for the connection.

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


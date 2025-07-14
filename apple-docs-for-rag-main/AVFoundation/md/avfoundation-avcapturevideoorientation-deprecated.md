

- AVFoundation
-  AVCaptureVideoOrientation Deprecated

Enumeration

# AVCaptureVideoOrientation

Constants indicating video orientation.

iOS 4.0–17.0DeprecatediPadOS 4.0–17.0DeprecatedMac Catalyst 14.0–17.0DeprecatedmacOS 10.7–14.0Deprecated

``` source
enum AVCaptureVideoOrientation
```

Deprecated

See videoRotationAngle instead.

## Overview

You can set these constants to videoOrientation for a connection that has an AVCaptureVideoPreviewLayer output.

## Topics

### Constants

case portrait

Indicates that video should be oriented vertically, top at the top.

case portraitUpsideDown

Indicates that video should be oriented vertically, top at the bottom.

case landscapeRight

Indicates that video should be oriented horizontally, top on the left.

case landscapeLeft

Indicates that video should be oriented horizontally, top on the right.

### Initializers

init?(rawValue: Int)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Deprecated

var isVideoStabilizationEnabled: Bool

A Boolean value that indicates whether video stabilization is active for the connection.

Deprecated

var enablesVideoStabilizationWhenAvailable: Bool

A Boolean value that indicates whether the system enables video stabilization when it’s available.

Deprecated

var isVideoOrientationSupported: Bool

A Boolean value that indicates whether the connection supports changing the orientation of the video.

Deprecated

var videoOrientation: AVCaptureVideoOrientation

An orientation that tells the connection how to rotate a video flowing through it.

Deprecated


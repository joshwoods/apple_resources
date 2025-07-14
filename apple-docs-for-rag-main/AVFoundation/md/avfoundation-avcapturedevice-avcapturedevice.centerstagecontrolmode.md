

- AVFoundation
- AVCaptureDevice
-  AVCaptureDevice.CenterStageControlMode 

Enumeration

# AVCaptureDevice.CenterStageControlMode

Constants that indicate the current Center Stage control mode.

iOS 14.5+iPadOS 14.5+Mac Catalyst 14.5+macOS 12.3+tvOS 17.0+

``` source
enum CenterStageControlMode
```

## Topics

### Control Modes

case user

The user controls Center Stage.

case app

The app controls Center Stage.

case cooperative

A user and app cooperatively share control of Center Stage.

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

### Configuring Center Stage

var isCenterStageActive: Bool

A Boolean value that indicates whether Center Stage is active on a device.

class var isCenterStageEnabled: Bool

A Boolean value that indicates whether a user or an app enabled Center Stage on a device.

var centerStageRectOfInterest: CGRect

The effective region within the output pixel buffer to perform Center Stage framing.

class var centerStageControlMode: AVCaptureDevice.CenterStageControlMode

A value that indicates the current mode of Center Stage control.


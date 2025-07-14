

- AVFoundation
- AVCaptureDevice
- AVCaptureDevice.CenterStageControlMode
-  AVCaptureDevice.CenterStageControlMode.user 

Case

# AVCaptureDevice.CenterStageControlMode.user

The user controls Center Stage.

iOS 14.5+iPadOS 14.5+Mac Catalyst 14.5+macOS 12.3+tvOS 17.0+

``` source
case user
```

## Discussion

In this mode, the user has exclusive control of Center Stage through Control Center. The system throws an exception in this mode if an app attempts to programmatically change the enabled state of Center Stage.

## See Also

### Control Modes

case app

The app controls Center Stage.

case cooperative

A user and app cooperatively share control of Center Stage.


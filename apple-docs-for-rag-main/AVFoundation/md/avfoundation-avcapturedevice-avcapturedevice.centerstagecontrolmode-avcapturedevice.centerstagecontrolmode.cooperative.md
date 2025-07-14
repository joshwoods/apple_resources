

- AVFoundation
- AVCaptureDevice
- AVCaptureDevice.CenterStageControlMode
-  AVCaptureDevice.CenterStageControlMode.cooperative 

Case

# AVCaptureDevice.CenterStageControlMode.cooperative

A user and app cooperatively share control of Center Stage.

iOS 14.5+iPadOS 14.5+Mac Catalyst 14.5+macOS 12.3+tvOS 17.0+

``` source
case cooperative
```

## Discussion

In this mode, it’s your app’s responsibilitiy to honor user intent and make center stage active when they request. Because the user can change the enabled state through Control Center, key-value observe the isCenterStageEnabled property value and update your app state appropriately.

## See Also

### Control Modes

case user

The user controls Center Stage.

case app

The app controls Center Stage.


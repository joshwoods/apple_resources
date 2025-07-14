

- AVFoundation
- AVCaptureDevice
- AVCaptureDevice.PrimaryConstituentDeviceRestrictedSwitchingBehaviorConditions
-  videoZoomChanged 

Type Property

# videoZoomChanged

Restrict switching to a fallback camera only when the device’s video zoom changes.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 17.0+

``` source
static var videoZoomChanged: AVCaptureDevice.PrimaryConstituentDeviceRestrictedSwitchingBehaviorConditions { get }
```

## Discussion

This condition switches cameras when the video zoom factor changes, either by setting a value for the device’s videoZoomFactor property or calling its ramp(toVideoZoomFactor:withRate:) method.

Note

All changes to video zoom factor allow switching to a fallback camera, not only those changes across switch-over zoom factors.

## See Also

### Switching Behavior Conditions

static var exposureModeChanged: AVCaptureDevice.PrimaryConstituentDeviceRestrictedSwitchingBehaviorConditions

Restrict switching to a fallback camera only when the device’s exposure mode changes.

static var focusModeChanged: AVCaptureDevice.PrimaryConstituentDeviceRestrictedSwitchingBehaviorConditions

Restrict switching to a fallback camera only when the device’s focus mode changes.


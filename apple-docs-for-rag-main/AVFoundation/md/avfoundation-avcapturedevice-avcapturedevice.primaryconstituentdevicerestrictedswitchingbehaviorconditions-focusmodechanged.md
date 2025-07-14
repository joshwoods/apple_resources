

- AVFoundation
- AVCaptureDevice
- AVCaptureDevice.PrimaryConstituentDeviceRestrictedSwitchingBehaviorConditions
-  focusModeChanged 

Type Property

# focusModeChanged

Restrict switching to a fallback camera only when the device’s focus mode changes.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 17.0+

``` source
static var focusModeChanged: AVCaptureDevice.PrimaryConstituentDeviceRestrictedSwitchingBehaviorConditions { get }
```

## See Also

### Switching Behavior Conditions

static var exposureModeChanged: AVCaptureDevice.PrimaryConstituentDeviceRestrictedSwitchingBehaviorConditions

Restrict switching to a fallback camera only when the device’s exposure mode changes.

static var videoZoomChanged: AVCaptureDevice.PrimaryConstituentDeviceRestrictedSwitchingBehaviorConditions

Restrict switching to a fallback camera only when the device’s video zoom changes.


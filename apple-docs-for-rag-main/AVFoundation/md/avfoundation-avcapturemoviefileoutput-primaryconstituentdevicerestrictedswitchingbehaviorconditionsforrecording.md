

- AVFoundation
- AVCaptureMovieFileOutput
-  primaryConstituentDeviceRestrictedSwitchingBehaviorConditionsForRecording 

Instance Property

# primaryConstituentDeviceRestrictedSwitchingBehaviorConditionsForRecording

The conditions during which camera switching may occur while recording.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 17.0+

``` source
var primaryConstituentDeviceRestrictedSwitchingBehaviorConditionsForRecording: AVCaptureDevice.PrimaryConstituentDeviceRestrictedSwitchingBehaviorConditions { get }
```

## Discussion

The default conditions include videoZoomChanged, focusModeChanged, and exposureModeChanged.

This property is key-value observable.

## See Also

### Restricting camera switching

var isPrimaryConstituentDeviceSwitchingBehaviorForRecordingEnabled: Bool

A Boolean value that indicates whether to restrict constituent device switching behavior during recording.

func setPrimaryConstituentDeviceSwitchingBehaviorForRecording(AVCaptureDevice.PrimaryConstituentDeviceSwitchingBehavior, restrictedSwitchingBehaviorConditions: AVCaptureDevice.PrimaryConstituentDeviceRestrictedSwitchingBehaviorConditions)

Sets the camera switching behavior to use during recording.

var primaryConstituentDeviceSwitchingBehaviorForRecording: AVCaptureDevice.PrimaryConstituentDeviceSwitchingBehavior

The camera switching behavior to use for recording.


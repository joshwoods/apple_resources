

- AVFoundation
- AVCaptureMovieFileOutput
-  primaryConstituentDeviceSwitchingBehaviorForRecording 

Instance Property

# primaryConstituentDeviceSwitchingBehaviorForRecording

The camera switching behavior to use for recording.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 17.0+

``` source
var primaryConstituentDeviceSwitchingBehaviorForRecording: AVCaptureDevice.PrimaryConstituentDeviceSwitchingBehavior { get }
```

## Discussion

The default value of this property is AVCaptureDevice.PrimaryConstituentDeviceSwitchingBehavior.restricted.

This property is key-value observable.

## See Also

### Restricting camera switching

var isPrimaryConstituentDeviceSwitchingBehaviorForRecordingEnabled: Bool

A Boolean value that indicates whether to restrict constituent device switching behavior during recording.

func setPrimaryConstituentDeviceSwitchingBehaviorForRecording(AVCaptureDevice.PrimaryConstituentDeviceSwitchingBehavior, restrictedSwitchingBehaviorConditions: AVCaptureDevice.PrimaryConstituentDeviceRestrictedSwitchingBehaviorConditions)

Sets the camera switching behavior to use during recording.

var primaryConstituentDeviceRestrictedSwitchingBehaviorConditionsForRecording: AVCaptureDevice.PrimaryConstituentDeviceRestrictedSwitchingBehaviorConditions

The conditions during which camera switching may occur while recording.


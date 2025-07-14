

- AVFoundation
- AVCaptureMovieFileOutput
-  setPrimaryConstituentDeviceSwitchingBehaviorForRecording(\_:restrictedSwitchingBehaviorConditions:) 

Instance Method

# setPrimaryConstituentDeviceSwitchingBehaviorForRecording(\_:restrictedSwitchingBehaviorConditions:)

Sets the camera switching behavior to use during recording.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 17.0+

``` source
func setPrimaryConstituentDeviceSwitchingBehaviorForRecording(
    _ switchingBehavior: AVCaptureDevice.PrimaryConstituentDeviceSwitchingBehavior,
    restrictedSwitchingBehaviorConditions: AVCaptureDevice.PrimaryConstituentDeviceRestrictedSwitchingBehaviorConditions
)
```

## Parameters 

`switchingBehavior`  

The switching behavior to set on the movie file output.

Attempting to restrict the switching behavior of a capture device that doesn’t support constituent device switching results in an error.

`restrictedSwitchingBehaviorConditions`  

The conditions during which camera switching occurs. Only set a condition when you set the switching behavior to AVCaptureDevice.PrimaryConstituentDeviceSwitchingBehavior.restricted. In all other cases, set the value to AVCapturePrimaryConstituentDeviceRestrictedSwitchingBehaviorConditionNone.

## Discussion

Use this method to control the camera switching behavior the system uses when recording a movie. The behavior you specify takes effect when you enable it by setting the value of isPrimaryConstituentDeviceSwitchingBehaviorForRecordingEnabled to true.

When a capture device doesn’t support constituent device selection, attempting to set a behavior other than AVCaptureDevice.PrimaryConstituentDeviceSwitchingBehavior.unsupported causes the system to throw an invalid argument exception.

## See Also

### Restricting camera switching

var isPrimaryConstituentDeviceSwitchingBehaviorForRecordingEnabled: Bool

A Boolean value that indicates whether to restrict constituent device switching behavior during recording.

var primaryConstituentDeviceSwitchingBehaviorForRecording: AVCaptureDevice.PrimaryConstituentDeviceSwitchingBehavior

The camera switching behavior to use for recording.

var primaryConstituentDeviceRestrictedSwitchingBehaviorConditionsForRecording: AVCaptureDevice.PrimaryConstituentDeviceRestrictedSwitchingBehaviorConditions

The conditions during which camera switching may occur while recording.


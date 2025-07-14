

- AVFoundation
- AVCaptureMovieFileOutput
-  isPrimaryConstituentDeviceSwitchingBehaviorForRecordingEnabled 

Instance Property

# isPrimaryConstituentDeviceSwitchingBehaviorForRecordingEnabled

A Boolean value that indicates whether to restrict constituent device switching behavior during recording.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 17.0+

``` source
var isPrimaryConstituentDeviceSwitchingBehaviorForRecordingEnabled: Bool { get set }
```

## Discussion

Use this property to enable camera switching restrictions when recording movies. You set restrictions by calling the output’s setPrimaryConstituentDeviceSwitchingBehaviorForRecording(_:restrictedSwitchingBehaviorConditions:) method. The restrictions take effect when you start recording, and revert to the behavior set by the capture device’s primaryConstituentDeviceSwitchingBehavior when you stop recording.

By default, this property is true when connected to a capture device that supports constituent device switching.

## See Also

### Restricting camera switching

func setPrimaryConstituentDeviceSwitchingBehaviorForRecording(AVCaptureDevice.PrimaryConstituentDeviceSwitchingBehavior, restrictedSwitchingBehaviorConditions: AVCaptureDevice.PrimaryConstituentDeviceRestrictedSwitchingBehaviorConditions)

Sets the camera switching behavior to use during recording.

var primaryConstituentDeviceSwitchingBehaviorForRecording: AVCaptureDevice.PrimaryConstituentDeviceSwitchingBehavior

The camera switching behavior to use for recording.

var primaryConstituentDeviceRestrictedSwitchingBehaviorConditionsForRecording: AVCaptureDevice.PrimaryConstituentDeviceRestrictedSwitchingBehaviorConditions

The conditions during which camera switching may occur while recording.


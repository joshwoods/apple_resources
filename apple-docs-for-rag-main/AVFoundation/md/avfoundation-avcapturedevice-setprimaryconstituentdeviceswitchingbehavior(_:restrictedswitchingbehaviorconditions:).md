

- AVFoundation
- AVCaptureDevice
-  setPrimaryConstituentDeviceSwitchingBehavior(\_:restrictedSwitchingBehaviorConditions:) 

Instance Method

# setPrimaryConstituentDeviceSwitchingBehavior(\_:restrictedSwitchingBehaviorConditions:)

Sets the switching behavior of the primary constituent device.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 17.0+

``` source
func setPrimaryConstituentDeviceSwitchingBehavior(
    _ switchingBehavior: AVCaptureDevice.PrimaryConstituentDeviceSwitchingBehavior,
    restrictedSwitchingBehaviorConditions: AVCaptureDevice.PrimaryConstituentDeviceRestrictedSwitchingBehaviorConditions
)
```

## Parameters 

`switchingBehavior`  

The switching behavior to set on the device.

`restrictedSwitchingBehaviorConditions`  

Sets the conditions during which the system restricts switching cameras.

Setting the switching behavior to a value other than AVCaptureDevice.PrimaryConstituentDeviceSwitchingBehavior.restricted requires that you set this argument to an empty option set.

## Discussion

Use this method to configure the camera switching behavior of a capture device. Before calling it, determine if a device supports configuring its device switching behavior by querying the device’s activePrimaryConstituentDeviceSwitchingBehavior property. If the value equals `.unsupported`, attempting to configure its switching behavior results in an error.

```
// Exit early if the device doesn't support configuring switching behavior.
guard captureDevice.activePrimaryConstituentDeviceSwitchingBehavior != .unsupported else { return }
captureDevice.setPrimaryConstituentDeviceSwitchingBehavior(.auto, restrictedSwitchingBehaviorConditions: [])
```

When recording using an instance of AVCaptureMovieFileOutput, you may override the switching behavior by calling the movie file output’s setPrimaryConstituentDeviceSwitchingBehaviorForRecording(_:restrictedSwitchingBehaviorConditions:) method.

## See Also

### Restricting Camera Switching

var primaryConstituentDeviceSwitchingBehavior: AVCaptureDevice.PrimaryConstituentDeviceSwitchingBehavior

The switching behavior for the primary constituent device.

var primaryConstituentDeviceRestrictedSwitchingBehaviorConditions: AVCaptureDevice.PrimaryConstituentDeviceRestrictedSwitchingBehaviorConditions

The conditions that restrict the primary constituent device’s switching behavior.

var activePrimaryConstituentDeviceSwitchingBehavior: AVCaptureDevice.PrimaryConstituentDeviceSwitchingBehavior

The switching behavior of the active constituent device.

var activePrimaryConstituentDeviceRestrictedSwitchingBehaviorConditions: AVCaptureDevice.PrimaryConstituentDeviceRestrictedSwitchingBehaviorConditions

The conditions that restrict camera switching behavior for the active primary constituent device.

var activePrimaryConstituent: AVCaptureDevice?

A virtual device’s active primary constituent device.

enum PrimaryConstituentDeviceSwitchingBehavior

Constants that control when to allow a virtual device to switch its active primary constituent device.

struct PrimaryConstituentDeviceRestrictedSwitchingBehaviorConditions

A structure that defines the conditions in which to restrict camera switching.

var supportedFallbackPrimaryConstituentDevices: [AVCaptureDevice]

The constituent devices available to select as a fallback for a longer focal length primary constituent device.

var fallbackPrimaryConstituentDevices: [AVCaptureDevice]

The fallback devices to use when a constituent device with a longer focal length becomes limited by its light sensitivity or minimum focus distance.


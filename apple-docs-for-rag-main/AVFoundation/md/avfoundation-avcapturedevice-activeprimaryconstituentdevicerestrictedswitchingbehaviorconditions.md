

- AVFoundation
- AVCaptureDevice
-  activePrimaryConstituentDeviceRestrictedSwitchingBehaviorConditions 

Instance Property

# activePrimaryConstituentDeviceRestrictedSwitchingBehaviorConditions

The conditions that restrict camera switching behavior for the active primary constituent device.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 17.0+

``` source
var activePrimaryConstituentDeviceRestrictedSwitchingBehaviorConditions: AVCaptureDevice.PrimaryConstituentDeviceRestrictedSwitchingBehaviorConditions { get }
```

## Discussion

For virtual devices with multiple constituent devices, this property returns the active restricted switching behavior conditions. This is equal to primaryConstituentDeviceRestrictedSwitchingBehaviorConditions except while recording using an AVCaptureMovieFileOutput that you configure with different restricted switching behavior conditions.

Devices that don’t support constituent device switching return AVCapturePrimaryConstituentDeviceRestrictedSwitchingBehaviorConditionNone.

This property is key-value observable.

## See Also

### Restricting Camera Switching

func setPrimaryConstituentDeviceSwitchingBehavior(AVCaptureDevice.PrimaryConstituentDeviceSwitchingBehavior, restrictedSwitchingBehaviorConditions: AVCaptureDevice.PrimaryConstituentDeviceRestrictedSwitchingBehaviorConditions)

Sets the switching behavior of the primary constituent device.

var primaryConstituentDeviceSwitchingBehavior: AVCaptureDevice.PrimaryConstituentDeviceSwitchingBehavior

The switching behavior for the primary constituent device.

var primaryConstituentDeviceRestrictedSwitchingBehaviorConditions: AVCaptureDevice.PrimaryConstituentDeviceRestrictedSwitchingBehaviorConditions

The conditions that restrict the primary constituent device’s switching behavior.

var activePrimaryConstituentDeviceSwitchingBehavior: AVCaptureDevice.PrimaryConstituentDeviceSwitchingBehavior

The switching behavior of the active constituent device.

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


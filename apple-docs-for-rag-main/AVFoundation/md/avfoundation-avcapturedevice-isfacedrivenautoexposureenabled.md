

- AVFoundation
- AVCaptureDevice
-  isFaceDrivenAutoExposureEnabled 

Instance Property

# isFaceDrivenAutoExposureEnabled

A Boolean value that indicates whether the device has face-driven autoexposure enabled.

iOS 15.4+iPadOS 15.4+Mac Catalyst 15.4+tvOS 17.0+

``` source
var isFaceDrivenAutoExposureEnabled: Bool { get set }
```

## Discussion

Face-driven autoexposure takes a subject’s face into account when performing automatic exposure adjustments. Enabling this feature can better expose subjects with darker skin tones or those who are backlit. For apps that link against iOS 15.4 or later, the value of this property defaults to true for devices that support autoexposure.

Before setting a value for this property, perform the following:

- Obtain exclusive access to the device by calling its lockForConfiguration() method.

- Set the value of the device’s automaticallyAdjustsFaceDrivenAutoExposureEnabled property to false.

Attempting to set a value before performing these steps results in an exception.

When you finish configuring the device, unlock it by calling its unlockForConfiguration() method.

Important

Updating the state of this property doesn’t initiate an exposure change. After setting a new value, set an appropriate exposureMode to apply the change.

## See Also

### Configuring Face-Driven Automatic Exposure

var automaticallyAdjustsFaceDrivenAutoExposureEnabled: Bool

A Boolean value that indicates whether the device automatically adjusts face-driven autoexposure.




- AVFoundation
- AVCaptureDevice
-  automaticallyAdjustsFaceDrivenAutoExposureEnabled 

Instance Property

# automaticallyAdjustsFaceDrivenAutoExposureEnabled

A Boolean value that indicates whether the device automatically adjusts face-driven autoexposure.

iOS 15.4+iPadOS 15.4+Mac Catalyst 15.4+tvOS 17.0+

``` source
var automaticallyAdjustsFaceDrivenAutoExposureEnabled: Bool { get set }
```

## Discussion

The value of this property defaults to true for devices that support autoexposure. If your app requires explicitly setting the state of isFaceDrivenAutoExposureEnabled, set this value to false.

To set this property value, you must call the device’s lockForConfiguration() method to obtain exclusive access to configure it. Otherwise, attempting to set a value raises an exception. When you finish configuring the device, call unlockForConfiguration() to release the lock.

## See Also

### Configuring Face-Driven Automatic Exposure

var isFaceDrivenAutoExposureEnabled: Bool

A Boolean value that indicates whether the device has face-driven autoexposure enabled.


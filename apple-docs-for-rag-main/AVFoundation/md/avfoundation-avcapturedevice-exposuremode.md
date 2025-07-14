

- AVFoundation
- AVCaptureDevice
-  exposureMode 

Instance Property

# exposureMode

The exposure mode for the device.

iOS 4.0+iPadOS 4.0+Mac Catalyst 14.0+macOS 10.7+tvOS 17.0+

``` source
var exposureMode: AVCaptureDevice.ExposureMode { get set }
```

## Discussion

Before changing the value of this property, you must call lockForConfiguration() to acquire exclusive access to the device’s configuration properties. Otherwise, setting the value of this property raises an exception. When you’re done configuring the device, call unlockForConfiguration() to release the lock and allow other devices to configure the settings.

This property is key-value observable.

## See Also

### Managing the Exposure Mode

func isExposureModeSupported(AVCaptureDevice.ExposureMode) -> Bool

Returns a Boolean value that indicates whether a device supports the specified exposure mode.

enum ExposureMode

Constants that specify the exposure mode of a capture device.


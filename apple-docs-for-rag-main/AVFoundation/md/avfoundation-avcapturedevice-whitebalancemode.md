

- AVFoundation
- AVCaptureDevice
-  whiteBalanceMode 

Instance Property

# whiteBalanceMode

The current white balance mode.

iOS 4.0+iPadOS 4.0+Mac Catalyst 14.0+macOS 10.7+tvOS 17.0+

``` source
var whiteBalanceMode: AVCaptureDevice.WhiteBalanceMode { get set }
```

## Discussion

Before changing the value of this property, you must call lockForConfiguration() to acquire exclusive access to the device’s configuration properties. Otherwise, setting the value of this property raises an exception. When you’re done configuring the device, call unlockForConfiguration() to release the lock and allow other devices to configure the settings.

This property is key-value observable.

## See Also

### Configuring Automatic White Balance

func isWhiteBalanceModeSupported(AVCaptureDevice.WhiteBalanceMode) -> Bool

Returns a Boolean value that indicates whether the device supports the specified white balance mode.

enum WhiteBalanceMode

Constants to specify the white balance mode of a capture device.


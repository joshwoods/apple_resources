

- AVFoundation
- AVCaptureDevice
-  flashMode Deprecated

Instance Property

# flashMode

The device’s current flash mode.

iOS 4.0–10.0DeprecatediPadOS 4.0–10.0DeprecatedMac Catalyst 13.1–13.1DeprecatedmacOS 10.7+

``` source
var flashMode: AVCaptureDevice.FlashMode { get set }
```

Deprecated

Use flashMode on AVCapturePhotoSettings instead.

## Discussion

Before changing the value of this property, you must call lockForConfiguration() to acquire exclusive access to the device’s configuration properties. Otherwise, setting the value of this property raises an exception. When you finish configuring the device, call unlockForConfiguration() to release the lock and allow other devices to configure the settings.

This property is key-value observable.

## See Also

### Configuring Flash Settings

var hasFlash: Bool

A Boolean value that indicates whether the capture device has a flash.

var isFlashAvailable: Bool

A Boolean value that indicates whether the flash is currently available for use.

var isFlashActive: Bool

A Boolean value that indicates whether the flash is currently active.

Deprecated

func isFlashModeSupported(AVCaptureDevice.FlashMode) -> Bool

Returns a Boolean value that indicates whether the device supports the given flash mode.

Deprecated

enum FlashMode

Constants that specify the flash modes of a capture device.


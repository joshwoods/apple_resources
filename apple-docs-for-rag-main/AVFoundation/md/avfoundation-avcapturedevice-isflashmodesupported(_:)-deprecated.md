

- AVFoundation
- AVCaptureDevice
-  isFlashModeSupported(\_:) Deprecated

Instance Method

# isFlashModeSupported(\_:)

Returns a Boolean value that indicates whether the device supports the given flash mode.

iOS 4.0–10.0DeprecatediPadOS 4.0–10.0DeprecatedMac Catalyst 13.1–13.1DeprecatedmacOS 10.7+

``` source
func isFlashModeSupported(_ flashMode: AVCaptureDevice.FlashMode) -> Bool
```

Deprecated

Use supportedFlashModes on AVCapturePhotoOutput instead.

## Parameters 

`flashMode`  

A flash mode to test if the device supports.

## Return Value

true if the device supports the flash mode; otherwise, false.

## See Also

### Configuring Flash Settings

var hasFlash: Bool

A Boolean value that indicates whether the capture device has a flash.

var isFlashAvailable: Bool

A Boolean value that indicates whether the flash is currently available for use.

var isFlashActive: Bool

A Boolean value that indicates whether the flash is currently active.

Deprecated

var flashMode: AVCaptureDevice.FlashMode

The device’s current flash mode.

Deprecated

enum FlashMode

Constants that specify the flash modes of a capture device.


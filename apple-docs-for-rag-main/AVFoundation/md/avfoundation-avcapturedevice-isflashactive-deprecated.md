

- AVFoundation
- AVCaptureDevice
-  isFlashActive Deprecated

Instance Property

# isFlashActive

A Boolean value that indicates whether the flash is currently active.

iOS 5.0–10.0DeprecatediPadOS 5.0–10.0DeprecatedMac Catalyst 13.1–13.1Deprecated

``` source
var isFlashActive: Bool { get }
```

Deprecated

Use isFlashScene on AVCapturePhotoOutput instead.

## Discussion

When the flash is active, it flashes when capturing a photo.

This property is key-value observable.

## See Also

### Configuring Flash Settings

var hasFlash: Bool

A Boolean value that indicates whether the capture device has a flash.

var isFlashAvailable: Bool

A Boolean value that indicates whether the flash is currently available for use.

var flashMode: AVCaptureDevice.FlashMode

The device’s current flash mode.

Deprecated

func isFlashModeSupported(AVCaptureDevice.FlashMode) -> Bool

Returns a Boolean value that indicates whether the device supports the given flash mode.

Deprecated

enum FlashMode

Constants that specify the flash modes of a capture device.


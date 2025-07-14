

- AVFoundation
- AVCaptureDevice
-  hasFlash 

Instance Property

# hasFlash

A Boolean value that indicates whether the capture device has a flash.

iOS 4.0+iPadOS 4.0+Mac Catalyst 14.0+macOS 10.7+tvOS 17.0+

``` source
var hasFlash: Bool { get }
```

## Discussion

This property is key-value observable.

## See Also

### Configuring Flash Settings

var isFlashAvailable: Bool

A Boolean value that indicates whether the flash is currently available for use.

var isFlashActive: Bool

A Boolean value that indicates whether the flash is currently active.

Deprecated

var flashMode: AVCaptureDevice.FlashMode

The device’s current flash mode.

Deprecated

func isFlashModeSupported(AVCaptureDevice.FlashMode) -> Bool

Returns a Boolean value that indicates whether the device supports the given flash mode.

Deprecated

enum FlashMode

Constants that specify the flash modes of a capture device.


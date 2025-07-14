

- AVFoundation
- AVCaptureDevice
-  isFlashAvailable 

Instance Property

# isFlashAvailable

A Boolean value that indicates whether the flash is currently available for use.

iOS 5.0+iPadOS 5.0+Mac Catalyst 14.0+macOS 10.15+tvOS 17.0+

``` source
var isFlashAvailable: Bool { get }
```

## Discussion

The flash may become unavailable if, for example, the device overheats and needs to cool off.

This property is key-value observable.

## See Also

### Configuring Flash Settings

var hasFlash: Bool

A Boolean value that indicates whether the capture device has a flash.

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


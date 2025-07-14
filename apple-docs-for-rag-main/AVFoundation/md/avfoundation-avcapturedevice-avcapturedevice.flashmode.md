

- AVFoundation
- AVCaptureDevice
-  AVCaptureDevice.FlashMode 

Enumeration

# AVCaptureDevice.FlashMode

Constants that specify the flash modes of a capture device.

iOS 4.0+iPadOS 4.0+Mac Catalyst 14.0+macOS 10.7+tvOS 17.0+

``` source
enum FlashMode
```

## Topics

### Flash Modes

case off

A mode that indicates the flash is off.

case on

A mode that indicates the flash is on.

case auto

A mode that indicates the device continuously monitors light levels and uses the flash when necessary.

### Initializers

init?(rawValue: Int)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

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

func isFlashModeSupported(AVCaptureDevice.FlashMode) -> Bool

Returns a Boolean value that indicates whether the device supports the given flash mode.

Deprecated


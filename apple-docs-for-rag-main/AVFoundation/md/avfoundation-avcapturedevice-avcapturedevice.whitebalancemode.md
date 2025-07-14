

- AVFoundation
- AVCaptureDevice
-  AVCaptureDevice.WhiteBalanceMode 

Enumeration

# AVCaptureDevice.WhiteBalanceMode

Constants to specify the white balance mode of a capture device.

iOS 4.0+iPadOS 4.0+Mac Catalyst 14.0+macOS 10.7+tvOS 17.0+

``` source
enum WhiteBalanceMode
```

## Topics

### White Balance Modes

case locked

A mode that locks the white balance state.

case autoWhiteBalance

A mode that automatically manages white balance.

case continuousAutoWhiteBalance

A mode that continuously monitors white balance and adjusts when necessary.

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

### Configuring Automatic White Balance

func isWhiteBalanceModeSupported(AVCaptureDevice.WhiteBalanceMode) -> Bool

Returns a Boolean value that indicates whether the device supports the specified white balance mode.

var whiteBalanceMode: AVCaptureDevice.WhiteBalanceMode

The current white balance mode.




- AVFoundation
- AVCaptureDevice
-  AVCaptureDevice.Position 

Enumeration

# AVCaptureDevice.Position

Constants that indicate the physical position of a capture device.

iOS 4.0+iPadOS 4.0+Mac Catalyst 14.0+macOS 10.7+tvOS 17.0+visionOS 1.0+

``` source
enum Position
```

## Topics

### Positions

case front

A position on the user-facing side of an iOS device.

case back

A position on the subject-facing side of an iOS device.

case unspecified

A position that’s unspecified.

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

### Identifying a Device

var uniqueID: String

An identifier that uniquely identifies the device.

var modelID: String

A model identifier for the device.

var localizedName: String

A localized device name for display in the user interface.

var manufacturer: String

A human-readable string for the manufacturer of the device.

var deviceType: AVCaptureDevice.DeviceType

The type of device, such as a built-in microphone or wide-angle camera.

struct DeviceType

A structure that defines the device types the framework supports.

var position: AVCaptureDevice.Position

The physical position of the capture device hardware.




- ImageCaptureCore
-  ICDeviceTypeMask 

Enumeration

# ICDeviceTypeMask

Masks for detecting different device types.

iOS 15.2+iPadOS 15.2+Mac Catalyst 15.2+macOS 10.4+visionOS 1.0+

``` source
enum ICDeviceTypeMask
```

## Topics

### Constants

case camera

A mask for detecting a camera.

case scanner

A mask for detecting a scanner.

### Initializers

init?(rawValue: UInt)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Inspecting a Device’s Type and Location

var type: ICDeviceType

A combination of the device’s type and its location type.

enum ICDeviceType

The type of image capture device.

var locationDescription: String?

A nonlocalized location description for the device.

var modulePath: String

The file system path of the device module associated with this device.

var moduleVersion: String?

The bundle version of the device module associated with this device.

enum ICDeviceLocationType

The location of the image capture device.

enum ICDeviceLocationTypeMask

Masks for detecting different device locations.

struct ICDeviceLocationOptions

Options for the location of the image capture device.

var usbLocationID: Int32

The USB location that the device is occupying.

var usbProductID: Int32

The USB Product ID (PID) associated with the device.

var usbVendorID: Int32

The USB Vendor ID (VID) associated with the device.


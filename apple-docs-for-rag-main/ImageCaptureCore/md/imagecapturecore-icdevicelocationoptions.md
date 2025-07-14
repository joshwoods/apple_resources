

- ImageCaptureCore
-  ICDeviceLocationOptions 

Structure

# ICDeviceLocationOptions

Options for the location of the image capture device.

iOSiPadOSMac CatalystmacOSvisionOS

``` source
struct ICDeviceLocationOptions
```

## Topics

### Creating Location Options

init(rawValue: String)

Creates ImageCaptureCore location options.

### Determining a Location

static let descriptionBluetooth: ICDeviceLocationOptions

A paired Bluetooth device.

static let descriptionFireWire: ICDeviceLocationOptions

A device that’s directly attached to the Mac through its FireWire port.

static let descriptionMassStorage: ICDeviceLocationOptions

A mass storage device.

static let descriptionUSB: ICDeviceLocationOptions

A device that’s directly attached to the Mac through its USB port.

## Relationships

### Conforms To

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

enum ICDeviceTypeMask

Masks for detecting different device types.

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

var usbLocationID: Int32

The USB location that the device is occupying.

var usbProductID: Int32

The USB Product ID (PID) associated with the device.

var usbVendorID: Int32

The USB Vendor ID (VID) associated with the device.


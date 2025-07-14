

- ImageCaptureCore
- ICDeviceBrowser
- ICDevice
-  moduleVersion 

Instance Property

# moduleVersion

The bundle version of the device module associated with this device.

macOS 10.4+

``` source
var moduleVersion: String? { get }
```

## Discussion

The bundle version may change if an existing device module associated with this device is updated or a new device module for this device is installed.

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


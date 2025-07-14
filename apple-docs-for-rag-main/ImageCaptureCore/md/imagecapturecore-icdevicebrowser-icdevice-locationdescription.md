

- ImageCaptureCore
- ICDeviceBrowser
- ICDevice
-  locationDescription 

Instance Property

# locationDescription

A nonlocalized location description for the device.

macOS 10.4+

``` source
var locationDescription: String? { get }
```

## Discussion

This property returns either the description of an ICDeviceLocationType, or a description obtained from the Bonjour `TXT` record of a network device.

## See Also

### Inspecting a Device’s Type and Location

var type: ICDeviceType

A combination of the device’s type and its location type.

enum ICDeviceType

The type of image capture device.

enum ICDeviceTypeMask

Masks for detecting different device types.

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


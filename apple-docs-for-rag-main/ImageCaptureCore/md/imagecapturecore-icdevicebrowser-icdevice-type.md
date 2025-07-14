

- ImageCaptureCore
- ICDeviceBrowser
- ICDevice
-  type 

Instance Property

# type

A combination of the device’s type and its location type.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.4+visionOS 1.0+

``` source
var type: ICDeviceType { get }
```

## Discussion

This property combines the device’s type, for example ICDeviceType.camera, with its location type, for example ICDeviceLocationType.bluetooth.

To isolate the device’s type, perform bitwise `AND` on this property with an ICDeviceTypeMask.

To isolate the device’s location type, perform bitwise `AND` on this property with an ICDeviceLocationTypeMask.

## See Also

### Inspecting a Device’s Type and Location

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

struct ICDeviceLocationOptions

Options for the location of the image capture device.

var usbLocationID: Int32

The USB location that the device is occupying.

var usbProductID: Int32

The USB Product ID (PID) associated with the device.

var usbVendorID: Int32

The USB Vendor ID (VID) associated with the device.




- Core HID
- HIDDeviceClient
-  descriptor 

Instance Property

# descriptor

The HID specification compliant report descriptor for the associated HID device.

macOS 15.0+

``` source
var descriptor: Data { get }
```

## Discussion

A report descriptor defines details about the device and the type of interactions that it can engage in, such as the type of input it can generate, and the requests it responds to. This is the raw descriptor in byte form. Information extracted from the report descriptor is available in other HIDDeviceClient properties.

For more details, see Human Interface Devices (HID) Specifications and Tools.

## See Also

### Get device information

var deviceUsages: [HIDUsage]

A convenient list of all the usages that the device supports.

var isBuiltIn: Bool

A Boolean value that determines whether the device is built-in to the system or an external peripheral.

var localizationCode: HIDDeviceLocalizationCode

A location code that specifies the HID compliant localization code, if there is one.

var locationID: UInt64?

The location ID for the device, if there is one.

var manufacturer: String?

The manufacturer of the device, if known.

var modelNumber: String?

The model number for the device, if known.

let primaryUsage: HIDUsage

The HID specification compliant usage for the device.

var product: String?

The product name for the device, if known.

let productID: UInt32

The product ID for the device.

var serialNumber: String?

The serial number of the device, if known.

var transport: HIDDeviceTransport?

The data transport for the device.

var uniqueID: String?

A unique ID for the device, if there is one.

let vendorID: UInt32

The vendor ID for the device.

var versionNumber: UInt64?

The version of the device, if known.

var elements: [HIDElement]

All HID elements associated with the device.


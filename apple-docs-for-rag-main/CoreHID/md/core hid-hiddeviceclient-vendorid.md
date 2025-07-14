

- Core HID
- HIDDeviceClient
-  vendorID 

Instance Property

# vendorID

The vendor ID for the device.

macOS 15.0+

``` source
final let vendorID: UInt32
```

## Discussion

The vendor ID designates the vendor that produced the device. It can be combined with productID to determine the exact device.

More information about vendor IDs can be found online. The vendor ID associated with a HID device is typically a USB vendor ID (see Information for Developers), but can be something else, such as a Bluetooth vendor ID (see Assigned Numbers in the Bluetooth specification).

## See Also

### Get device information

var descriptor: Data

The HID specification compliant report descriptor for the associated HID device.

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

var versionNumber: UInt64?

The version of the device, if known.

var elements: [HIDElement]

All HID elements associated with the device.


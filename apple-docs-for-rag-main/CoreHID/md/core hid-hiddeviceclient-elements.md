

- Core HID
- HIDDeviceClient
-  elements 

Instance Property

# elements

All HID elements associated with the device.

macOS 15.0+

``` source
var elements: [HIDElement] { get }
```

## Discussion

Elements of interest can be taken from this list and passed to monitorNotifications(reportIDsToMonitor:elementsToMonitor:) to receive notifications using HIDDeviceClient.Notification.elementUpdates(values:) when updates to the elements are received from the device. Elements can also be used in a HIDDeviceClient.RequestElementUpdate to request the latest data as desired.

See HIDElement for more info.

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

let vendorID: UInt32

The vendor ID for the device.

var versionNumber: UInt64?

The version of the device, if known.




- Core HID
- HIDDeviceManager
- HIDDeviceManager.DeviceMatchingCriteria
-  vendorID 

Instance Property

# vendorID

The vendor ID for the device.

macOS 15.0+

``` source
var vendorID: UInt32?
```

## Discussion

The vendor ID designates the vendor that produced the device. Combine the vendor ID with the productID to determine the exact device.

More information about vendor IDs can be found online. The vendor ID associated with a HID device is typically a USB vendor ID (see Information for Developers), but can be something else, such as a Bluetooth vendor ID (see Assigned Numbers in the Bluetooth specification).


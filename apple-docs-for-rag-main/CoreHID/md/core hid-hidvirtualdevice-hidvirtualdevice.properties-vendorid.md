

- Core HID
- HIDVirtualDevice
- HIDVirtualDevice.Properties
-  vendorID 

Instance Property

# vendorID

The vendor ID for the device.

macOS 15.0+

``` source
let vendorID: UInt32
```

## Mentioned in 

Creating virtual devices

## Discussion

The vendor ID designates the vendor that produced the device. It can be combined with productID to determine the exact device.

More information about vendor IDs can be found online. The vendor ID associated with a HID device is typically a USB vendor ID, but can be something else, such as a Bluetooth vendor ID.


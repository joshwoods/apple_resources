

- Core HID
- HIDVirtualDevice
- HIDVirtualDevice.Properties
-  uniqueID 

Instance Property

# uniqueID

A unique ID for the device.

macOS 15.0+

``` source
let uniqueID: String?
```

## Discussion

Use `uniqueID` to facilitate driver matching, or client matching using HIDDeviceManager.


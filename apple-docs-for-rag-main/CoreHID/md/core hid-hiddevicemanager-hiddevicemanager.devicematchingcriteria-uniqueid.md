

- Core HID
- HIDDeviceManager
- HIDDeviceManager.DeviceMatchingCriteria
-  uniqueID 

Instance Property

# uniqueID

A unique ID for the device.

macOS 15.0+

``` source
var uniqueID: String?
```

## Discussion

This ID is software based, and isn’t associated with the device itself. It is typically set to help facilitate driver or client matching.


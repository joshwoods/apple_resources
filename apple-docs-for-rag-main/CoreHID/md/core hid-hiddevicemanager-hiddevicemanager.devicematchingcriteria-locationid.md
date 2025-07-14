

- Core HID
- HIDDeviceManager
- HIDDeviceManager.DeviceMatchingCriteria
-  locationID 

Instance Property

# locationID

The location ID for the device.

macOS 15.0+

``` source
var locationID: UInt64?
```

## Discussion

Location IDs are typically associated with USB devices, but can be overriden to have device implementation specific meaning.


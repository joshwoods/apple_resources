

- Core HID
- HIDDeviceManager
- HIDDeviceManager.DeviceMatchingCriteria
-  primaryUsage 

Instance Property

# primaryUsage

The HID specification compliant usage for the device.

macOS 15.0+

``` source
var primaryUsage: HIDUsage?
```

## Discussion

This is the main usage for the device, pulled from the top level collection of the report descriptor, specifying the general device type.

For more details, see HIDUsage.


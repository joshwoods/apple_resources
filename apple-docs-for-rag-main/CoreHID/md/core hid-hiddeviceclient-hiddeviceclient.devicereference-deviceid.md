

- Core HID
- HIDDeviceClient
- HIDDeviceClient.DeviceReference
-  deviceID 

Instance Property

# deviceID

The unique ID for the associated HID device.

macOS 15.0+

``` source
let deviceID: UInt64
```

## Discussion

A HIDDeviceClient.DeviceReferencewith the same deviceID is an equivalent reference to the same device, and a deviceID for a device is equivalent across the system.


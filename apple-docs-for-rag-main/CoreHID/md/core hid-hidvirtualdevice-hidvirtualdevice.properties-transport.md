

- Core HID
- HIDVirtualDevice
- HIDVirtualDevice.Properties
-  transport 

Instance Property

# transport

The data transport for the device.

macOS 15.0+

``` source
let transport: HIDDeviceTransport?
```

## Discussion

The data transport is typically HIDDeviceTransport.virtual, but it can be any HIDDeviceTransport.


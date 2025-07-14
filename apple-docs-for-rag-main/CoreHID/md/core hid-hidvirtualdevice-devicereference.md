

- Core HID
- HIDVirtualDevice
-  deviceReference 

Instance Property

# deviceReference

The reference to the virtual HID device.

macOS 15.0+

``` source
nonisolated
final let deviceReference: HIDDeviceClient.DeviceReference
```

## Discussion

Use to create a HIDDeviceClient, if creating a device and monitoring it within the same app is desired. For more details, see HIDDeviceClient.DeviceReference.

## See Also

### Create a HID virtual device

init?(properties: HIDVirtualDevice.Properties)

Creates a virtual HID device.

func activate(delegate: any HIDVirtualDeviceDelegate)

Activate a newly created virtual device to begin receiving notifications and enable functionality.


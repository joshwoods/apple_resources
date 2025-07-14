

- Core HID
- HIDDeviceClient
-  deviceReference 

Instance Property

# deviceReference

The reference to the HID device used to create the HID client device.

macOS 15.0+

``` source
nonisolated
final let deviceReference: HIDDeviceClient.DeviceReference
```

## Discussion

For more details, see HIDDeviceClient.DeviceReference.

## See Also

### Create a device client

init?(deviceReference: HIDDeviceClient.DeviceReference)

Creates a client for a HID device.

struct DeviceReference

A reference to a HID device on the system.


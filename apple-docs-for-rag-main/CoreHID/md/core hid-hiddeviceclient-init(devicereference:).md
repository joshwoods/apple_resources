

- Core HID
- HIDDeviceClient
-  init(deviceReference:) 

Initializer

# init(deviceReference:)

Creates a client for a HID device.

macOS 15.0+

``` source
init?(deviceReference: HIDDeviceClient.DeviceReference)
```

## Parameters 

`deviceReference`  

The reference to the target HID device that arrive using HIDDeviceManager. For more details, see HIDDeviceClient.DeviceReference.

## Discussion

After creating a HIDDeviceClient, notifications about the associated device arrive in monitorNotifications(reportIDsToMonitor:elementsToMonitor:).

## See Also

### Create a device client

struct DeviceReference

A reference to a HID device on the system.

let deviceReference: HIDDeviceClient.DeviceReference

The reference to the HID device used to create the HID client device.


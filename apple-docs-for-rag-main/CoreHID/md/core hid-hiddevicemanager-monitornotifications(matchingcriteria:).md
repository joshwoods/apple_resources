

- Core HID
- HIDDeviceManager
-  monitorNotifications(matchingCriteria:) 

Instance Method

# monitorNotifications(matchingCriteria:)

Creates an asynchronous stream that receives notifications for devices of interest.

macOS 15.0+

``` source
func monitorNotifications(matchingCriteria: [HIDDeviceManager.DeviceMatchingCriteria]) -> AsyncThrowingStream
```

## Parameters 

`matchingCriteria`  

A set of HIDDeviceManager.DeviceMatchingCriteria for matching devices connected to the system. Criteria are considered separately, if one set is specified that matches one device, with a second set that matches five other devices, all six devices are matched. Matched devices result in a HIDDeviceManager.Notification.deviceMatched(_:) notification. Matched devices are ready for connections using HIDDeviceClient until a HIDDeviceManager.Notification.deviceRemoved(_:) notification is received for the device.

## Return Value

An asynchronous stream that receives notifications.

## Mentioned in 

Communicating with human interface devices

## Discussion

Notifications come in asynchronously from the manager at arbitrary times when relevant events occur.

Example usage:

```
let searchCriteria = HIDDeviceManager.DeviceMatchingCriteria(primaryUsage: .genericDesktop(.keyboard), isBuiltIn: false)
for await notification in await manager.monitorNotifications(matchingCriteria: [searchCriteria]) {
    switch notification {
    case .deviceMatched(let deviceReference):
        client = HIDDeviceClient(deviceReference: deviceReference)
        break
    case .deviceRemoved(_):
        continue
    }
}
```

Throws

HIDDeviceError if there is an issue with setup.

## See Also

### Monitor device notifications

enum Notification

Notifications for HID devices.


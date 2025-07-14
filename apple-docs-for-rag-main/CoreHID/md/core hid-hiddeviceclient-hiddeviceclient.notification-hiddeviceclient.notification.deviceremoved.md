

- Core HID
- HIDDeviceClient
- HIDDeviceClient.Notification
-  HIDDeviceClient.Notification.deviceRemoved 

Case

# HIDDeviceClient.Notification.deviceRemoved

A notification that the device is no longer connected to the system.

macOS 15.0+

``` source
case deviceRemoved
```

## Discussion

After the device is removed, no other notifications occur and most methods fail. Discard the HIDDeviceClient.


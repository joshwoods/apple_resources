

- Core HID
- HIDDeviceManager
- HIDDeviceManager.Notification
-  HIDDeviceManager.Notification.deviceRemoved(\_:) 

Case

# HIDDeviceManager.Notification.deviceRemoved(\_:)

A notification that a previously matched device was removed from the system.

macOS 15.0+

``` source
case deviceRemoved(HIDDeviceClient.DeviceReference)
```

## Discussion

Any created HIDDeviceClient also receives a HIDDeviceClient.Notification.deviceRemoved notification.


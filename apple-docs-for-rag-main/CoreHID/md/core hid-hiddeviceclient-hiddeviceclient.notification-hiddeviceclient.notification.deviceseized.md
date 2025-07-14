

- Core HID
- HIDDeviceClient
- HIDDeviceClient.Notification
-  HIDDeviceClient.Notification.deviceSeized 

Case

# HIDDeviceClient.Notification.deviceSeized

A notification that the device was seized by another client.

macOS 15.0+

``` source
case deviceSeized
```

## Discussion

After the device is seized by another client, notifications are paused until HIDDeviceClient.Notification.deviceUnseized is received.


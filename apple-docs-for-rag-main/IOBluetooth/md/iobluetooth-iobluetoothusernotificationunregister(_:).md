

- IOBluetooth
-  IOBluetoothUserNotificationUnregister(\_:) 

Function

# IOBluetoothUserNotificationUnregister(\_:)

Unregisters the target notification.

macOS

``` source
func IOBluetoothUserNotificationUnregister(_ notificationRef: IOBluetoothUserNotificationRef!)
```

## Parameters 

`notificationRef`  

The target IOBluetoothUserNotificationRef to be unregistered

## Discussion

This function will unregister the notification. Once the notification has been unregistered, it will no longer call the callback. Additionally, once this function has been called the target IOBluetoothUserNotificationRef is no longer valid.

## See Also

### Miscellaneous

func IOBluetoothIgnoreHIDDevice(IOBluetoothDeviceRef!)

Hints that the macOS Bluetooth software should ignore a HID device that connects up.

func IOBluetoothL2CAPChannelRegisterForChannelCloseNotification(IOBluetoothL2CAPChannelRef!, IOBluetoothUserNotificationCallback!, UnsafeMutableRawPointer!) -> Unmanaged&lt;IOBluetoothUserNotificationRef>!

Allows a client to register for a channel close notification.

func IOBluetoothRemoveIgnoredHIDDevice(IOBluetoothDeviceRef!)

The counterpart to the above IOBluetoothIgnoreHIDDevice() API.

